<h2 align="center"> !!! Vue.js Interview Questions !!! </h2>

### Table of Contents

---

| No. | Questions                                                                           |
| --- | ----------------------------------------------------------------------------------- |
| 1   | [What is VueJS](#what-is-vuejs)                                                     |
| 2   | [What are the major features of VueJS](#what-are-the-major-features-of-vuejs)       |
| 3   | [What are the lifecycle methods of VueJS](#what-are-the-lifecycle-methods-of-vuejs) |

1.  ### What is VueJS?

    **Vue.js** is an open-source, progressive Javascript framework for building user interfaces that aim to be incrementally adoptable. The core library of VueJS is focused on the `view layer` only, and is easy to pick up and integrate with other libraries or existing projects.

    **[⬆ Back to Top](#table-of-contents)**

2.  ### What are the major features of VueJS?

    Below are the some of major features available with VueJS

    1. **Virtual DOM:** It uses virtual DOM similar to other existing frameworks such as ReactJS, Ember etc. Virtual DOM is a light-weight in-memory tree representation of the original HTML DOM and updated without affecting the original DOM.
    2. **Components:** Used to create reusable custom elements in VueJS applications.
    3. **Templates:** VueJS provides HTML based templates that bind the DOM with the Vue instance data
    4. **Routing:** Navigation between pages is achieved through vue-router
    5. **Light weight:** VueJS is light weight library compared to other frameworks.

    **[⬆ Back to Top](#table-of-contents)**

3.  ### What are the lifecycle methods of VueJS?

    Lifecycle hooks are a window into how the library you’re using works behind-the-scenes. By using these hooks, you will know when your component is created, added to the DOM, updated, or destroyed. Let's look at lifecycle diagram before going to each lifecycle hook in detail,

    <img src="https://github.com/sudheerj/vuejs-interview-questions/blob/master/images/lifecycle.png" width="400" height="800">

    1. **Creation(Initialization):**
       Creation Hooks allow you to perform actions before your component has even been added to the DOM. You need to use these hooks if you need to set things up in your component both during client rendering and server rendering. Unlike other hooks, creation hooks are also run during server-side rendering.
       1. beforeCreate:
          This hook runs at the very initialization of your component. hook observes data and initialization events in your component. Here, data is still not reactive and events that occur during the component’s lifecycle have not been set up yet.
       ```javascript
       new Vue({
         data: {
           count: 10,
         },
         beforeCreate: function () {
           console.log("Nothing gets called at this moment");
           // `this` points to the view model instance
           console.log("count is " + this.count);
         },
       });
       // count is undefined
       ```
       2. created:
          This hook is invoked when Vue has set up events and data observation. Here, events are active and access to reactive data is enabled though templates have not yet been mounted or rendered.
       ```javascript
       new Vue({
         data: {
           count: 10,
         },
         created: function () {
           // `this` points to the view model instance
           console.log("count is: " + this.count);
         },
       });
       // count is: 10
       ```
       **Note:** Remember that, You will not have access to the DOM or the target mounting element (this.$el) inside of creation hooks
    2. **Mounting(DOM Insertion):**
       Mounting hooks are often the most-used hooks and they allow you to access your component immediately before and after the first render.
       1. beforeMount:
          The beforeMount allows you to access your component immediately before and after the first render.
       ```javascript
       new Vue({
         beforeMount: function () {
           // `this` points to the view model instance
           console.log(`this.$el is yet to be created`);
         },
       });
       ```
       2. mounted:
          This is a most used hook and you will have full access to the reactive component, templates, and rendered DOM (via. this.$el). The most frequently used patterns are fetching data for your component.
       ```javascript
       <div id="app">
           <p>I’m text inside the component.</p>
       </div>
         new Vue({
           el: ‘#app’,
           mounted: function() {
             console.log(this.$el.textContent); // I'm text inside the component.
           }
         })
       ```
    3. **Updating (Diff & Re-render):**
       Updating hooks are called whenever a reactive property used by your component changes, or something else causes it to re-render

       1. beforeUpdate:
          The beforeUpdate hook runs after data changes on your component and the update cycle begins, right before the DOM is patched and re-rendered.

       ```javascript
       <div id="app">
         <p>{{counter}}</p>
       </div>
       ...// rest of the code
         new Vue({
           el: '#app',
           data() {
             return {
               counter: 0
             }
           },
            created: function() {
             setInterval(() => {
               this.counter++
             }, 1000)
           },

           beforeUpdate: function() {
             console.log(this.counter) // Logs the counter value every second, before the DOM updates.
           }
         })
       ```

       2. updated:
          This hook runs after data changes on your component and the DOM re-renders.

       ```javascript
       <div id="app">
         <p ref="dom">{{counter}}</p>
       </div>
       ...//
         new Vue({
           el: '#app',
           data() {
             return {
               counter: 0
             }
           },
            created: function() {
             setInterval(() => {
               this.counter++
             }, 1000)
           },
           updated: function() {
             console.log(+this.$refs['dom'].textContent === this.counter) // Logs true every second
           }
         })
       ```

    4. **Destruction (Teardown):**
       Destruction hooks allow you to perform actions when your component is destroyed, such as cleanup or analytics sending.

       1. beforeDestroy:
          `beforeDestroy` is fired right before teardown. If you need to cleanup events or reactive subscriptions, beforeDestroy would probably be the time to do it. Your component will still be fully present and functional.

       ```javascript
       new Vue({
         data() {
           return {
             message: "Welcome VueJS developers",
           };
         },

         beforeDestroy: function () {
           this.message = null;
           delete this.message;
         },
       });
       ```

       2. destroyed:
          This hooks is called after your component has been destroyed, its directives have been unbound and its event listeners have been removed.

       ```javascript
       new Vue({
         destroyed: function () {
           console.log(this); // Nothing to show here
         },
       });
       ```

    **[⬆ Back to Top](#table-of-contents)**
