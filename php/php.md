<h2 align="center"> !!! PHP Interview Questions !!! </h2>

### Table of Contents

---

| No. | Questions                                                                                                                                           |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What is PHP?](#what-is-PHP)                                                                                                                        |
| 2   | [What is PEAR in PHP?](#what-is-pear-in-php)                                                                                                        |
| 3   | [What is the name of scripting engine in PHP?](#what-is-the-name-of-scripting-engine-in-php)                                                        |
| 4   | [What is the difference between "echo", "print", "print_r" and "var_dump"?](#what-is-the-difference-between-echo-print-print_r-and-var_dump-in-PHP) |
| 5   | [What is the difference between `$message` and `$$message`?](#what-is-the-difference-between-$message-and-$$message-in-PHP)                         |
| 6   | [Explain the different types of errors in PHP !](#explain-the-different-types-of-errors-in-php)                                                     |
| 7   | [How many data types are there in PHP?](#how-many-data-types-are-there-in-php)                                                                      |
| 8   | [What is the use of header() function in PHP?](#what-is-the-use-of-header-function-in-php)                                                          |
| 9   | [How many types of array are there in PHP?](#how-many-types-of-array-are-there-in-php)                                                              |
| 10  | [Explain some of the PHP array functions?](#explain-some-of-the-PHP-array-functions)                                                                |
| 11  | [ Explain some of the PHP string functions?](#explain-some-of-the-PHP-string-functions)                                                             |
| 12  | [Differentiate between require and include?](#differentiate-between-require-and-include)                                                            |
| 13  | [Explain PHP Variables Scope?](#explain-php-variables-scope)                                                                                        |
| 14  | [Explain PHP Superglobals variables?](#explain-php-superglobals-variables)                                                                          |
| 15  | [What are the ways to define a constant in PHP?](#what-are-the-ways-to-define-a-constant-in-php)                                                    |
| 16  | [What is autoloading in php?](#what-is-autoloading-in-php)                                                                                          |
| 17  | [What is the difference between == and ===?](#what-is-the-difference-between-==-and-===)                                                            |
| 18  | [What is magic number in PHP?](#what-is-magic-number-in-php)                                                                                        |
| 19  | [What is htmlspecialchars in php?](#what-is-htmlspecialchars-in-php)                                                                                |
| 20  | [What is the use of DIR in PHP?](#what-is-the-use-of-dir-in-php)                                                                                    |
| 21  | [What is the purpose of the extract() function?](#what-is-the-purpose-of-the-extract-function)                                                      |
| 22  | [What is compact() function in PHP?](#what-is-compact-function-in-php)                                                                              |
| 23  | [What are the advantages of using namespaces in PHP?](#what-are-the-advantages-of-using-namespaces-in-php)                                          |
| 24  | [What does call_user_func() do in PHP?](#what-does-call_user_func-do-in-php)                                                                        |
| 25  | [What is the use of session in PHP?](#what-is-the-use-of-session-in-php)                                                                            |
| 26  | [What are the cookies in PHP?](#what-are-the-cookies-in-php)                                                                                        |
| 27  | [What does session_get_cookie_params() do in PHP?](#what-does-session_get_cookie_params-do-in-php)                                                  |
| 28  | [What does session_regenerate_id() do in PHP?](#what-does-session_regenerate_id-do-in-php)                                                          |
| 29  | [What is the difference between unset() and unlink()?](#what-is-the-difference-between-unset-and-unlink)                                            |
| 30  | [What is the difference between new self and new static in PHP?](#what-is-the-difference-between-new-self-and-new-static-in-php)                    |
| 31  | [What is the exception handling in PHP?](#what-is-the-exception-handling-in-php)                                                                    |
| 32  | [What does HTTP_REFERER do in PHP?](#what-does-http_referer-do-in-php)                                                                              |
| 33  | [What are magic methods and how to use them in PHP ?](#what-are-magic-methods-and-how-to-use-them-in-php)                                           |
| 34  | [What is ReflectionClass class in PHP?](#what-is-reflectionclass-class-in-php)                                                                      |
| 35  | [What is ReflectionMethod class in PHP?](#what-is-reflectionmethod-class-in-php)                                                                    |
| 36  | [What is the use of sscanf in PHP?](#what-is-the-use-of-sscanf-in-php)                                                                              |
| 37  | [What does list() do in PHP?](#what-does-list-do-in-php)                                                                                            |

1.  ### What is PHP?

    **PHP** stands for Hypertext Preprocessor. It is an open source server-side scripting language which is widely used for web development.

    **[⬆ Back to Top](#table-of-contents)**

2.  ### What is PEAR in PHP?

    **PEAR** stands for PHP Extension and Application Repository. It extends PHP and provides a higher level of programming for web developers.
    It contains all types of PHP code snippets and libraries. It also provides a command-line interface to install "packages" automatically.

    **[⬆ Back to Top](#table-of-contents)**

3.  ### What is the name of scripting engine in PHP?

    The scripting engine in PHP is called Zend Engine. It provides PHP with the ability to run scripts efficiently and quickly.

    **[⬆ Back to Top](#table-of-contents)**

4.  ### What is the difference between "Echo", "Print", "Print_r" and "Var_dump"?

    **Echo** and **print** are more or less the same. They are both used to output data to the screen.

    The differences are small: **echo** has no return value while **print** has a return value of 1 so it can be used in expressions. **echo** can take multiple parameters (although such usage is rare) while **print** can take one argument. **echo** is marginally faster than **print**.

    **print_r** displays information about a variable in a way that's readable by humans. **print_r** is used to print human-readable information about a variable, while **var_dump** is used to dump structural information about a variable that's more targeted towards developers.

    **Example :**

    ```
     echo "Hello, ", "World!"; //Output: Hello, World!

     print "Hello, World!"; //Output: Hello, World!

     $fruits = array("apple", "banana", "orange");

     print_r($fruits); //Output: Array ( [0] => apple [1] => banana [2] => orange )

     var_dump($fruits); //Output: array(3) { [0]=> string(5) "apple" [1]=> string(6) "banana" [2]=> string(6) "orange" }

    ```

    **[⬆ Back to Top](#table-of-contents)**

5.  ### What is the difference between `$message` and `$$message`?

    The **$message** (single dollar) is a normal variable with the name message that stores any value like string, integer, float, etc.

    The **$$message** (double dollar) is a reference variable that stores the value of the $message inside it.

    **Example :**

    ```
    $message = 'hello';
    $hello = 'world';

    echo $message; // Outputs: hello
    echo $$message; // Outputs: world

    ```

    **[⬆ Back to Top](#table-of-contents)**

6.  ### Explain the different types of errors in PHP !

    There are three types of errors:

    1. **Notices** : These are trivial, non-critical errors that PHP encounters while executing a script - for example, accessing a variable that has not yet been defined. By default, such errors are not displayed to the user at all - although you can change this default behavior.

    2. **Warnings** : These are more serious errors - for example, attempting to include() a file which does not exist. By default, these errors are displayed to the user, but they do not result in script termination.

    3. **Fatal errors** : These are critical errors - for example, instantiating an object of a non-existent class, or calling a non-existent function. These errors cause the immediate termination of the script, and PHP's default behavior is to display them to the user when they take place.

    **[⬆ Back to Top](#table-of-contents)**

7.  ### How many data types are there in PHP?

    **PHP** data types are used to hold different types of data or values. There are 8 primitive data types which are further categorized in 3 types:

    1. Scalar data types
    2. Compound data types
    3. Special data types

    **Scalar data types** : Scalar data types are those which can hold only a single value. There are 4 scalar data types:

    1. Boolean
    2. Integer
    3. Float
    4. String

    **Compound data types** : Compound data types are those which can hold multiple values and are further categorized in 2 types:

    1. Array
    2. Object

    **Special data types** : Special data types are those which can hold special values and are further categorized in 2 types:

    1. Resource
    2. NULL

    **[⬆ Back to Top](#table-of-contents)**

8.  ### What is the use of header() function in PHP?

    The **header()** function is used to send a raw HTTP header to a client. It must be called before sending the actual output, otherwise it will result in an error.

    **Example :**

    ```
     <?php
       header('Location: http://www.example.com/');
       exit;
      ?>

    ```

    **[⬆ Back to Top](#table-of-contents)**

9.  ### How many types of array are there in PHP?

    There are 3 types of array in PHP:

    1. **Indexed array** : An array with a numeric index. Values are stored and accessed in linear fashion.

    2. **Associative array** : An array with strings as index. This stores element values in association with key values rather than in a strict linear index order.

    3. **Multidimensional array** : An array containing one or more arrays and values are accessed using multiple indices.

    **Example :**

    ```
    $indexed_array = array("HTML", "CSS", "PHP");

    $associative_array = array(
        "HTML"=>"Hyper Text Markup Language",
        "CSS"=>"Cascading Style Sheet",
        "PHP"=>"Hypertext Preprocessor"
        );

    $multidimensional_array = array(
        "HTML"=>array("Hyper Text Markup Language", "Markup Language"),
        "CSS"=>array("Cascading Style Sheet", "Style Sheet Language"),
        "PHP"=>array("Hypertext Preprocessor", "Server Side Scripting Language")
        );

    ```

    **[⬆ Back to Top](#table-of-contents)**

10. ### Explain some of the PHP array functions?

    1. **array_push()**: This function is used to insert new items at the end of an array.

       ```
       <?php
         $fruits = array("apple", "banana");
         array_push($fruits, "cherry", "date");
         print_r($fruits);
       ?>
       ```

    2. **array_pop()**: This function removes the last element of an array.

       ```
       <?php
         $fruits = array("apple", "banana", "cherry");
         $lastFruit = array_pop($fruits);
         echo $lastFruit;
        ?>
       ```

    3. **array_shift()**: This function removes the first element of an array.

       ```
       <?php
         $fruits = array("apple", "banana", "cherry");
         $firstFruit = array_shift($fruits);
         echo $firstFruit;
       ?>
       ```

    4. **array_unshift()**: This function inserts new items at the beginning of an array

       ```
       <?php
        $fruits = array("banana", "cherry");
        array_unshift($fruits, "apple");
        print_r($fruits);
       ?>
       ```

    5. **count()**: This function is used to count all elements in an array.

       ```
       <?php
        $fruits = array("apple", "banana", "cherry");
        echo count($fruits);
       ?>
       ```

    6. **sort()**: This function sorts an array in ascending order.

       ```
       <?php
         $fruits = array("cherry", "banana", "apple");
         sort($fruits);
         print_r($fruits);
       ?>
       ```

    7. **rsort()**: This function sorts an array in descending order.

       ```
       <?php
         $fruits = array("apple", "banana", "cherry");
         rsort($fruits);
         print_r($fruits);
       ?>
       ```

    8. **array_merge()**: This function merges one or more arrays into one array.

       ```
       <?php
         $array1 = array("apple", "banana");
         $array2 = array("cherry", "date");
         $mergedArray = array_merge($array1, $array2);
         print_r($mergedArray);
       ?>
       ```

    9. **in_array()**: This function checks if a value exists in an array.

       ```

       <?php
         $fruits = array("apple", "banana", "cherry");
         if (in_array("banana", $fruits))
         {
             echo "Banana is in the array.";
         }
         else
         {
            echo "Banana is not in the array.";
         }
       ?>

       ```

    10. **array_keys()**: This function returns all the keys of an array.

        ```
        <?php
          $fruits = array("fruit1" => "apple", "fruit2" => "banana", "fruit3" => "cherry");
          $keys = array_keys($fruits);
          print_r($keys);
        ?>
        ```

    11. **array_values()**: This function returns all the values of an array.

        ```
        <?php
          $fruits = array("fruit1" => "apple", "fruit2" => "banana", "fruit3" => "cherry");
          $values = array_values($fruits);
          print_r($values);
        ?>
        ```

    12. **array_sum()**: This function returns the sum of all the values in an array.

        ```
        <?php
          $numbers = array(1, 2, 3, 4, 5);
          echo array_sum($numbers);
        ?>
        ```

    13. **array_map()**: This function sends each value of an array to a user-made function, and returns an array with new values, given by the user-made function.

        ```
        <?php
          function myfunction($value)
          {
            return($value*$value);
          }

          $a=array(1,2,3,4,5);
          print_r(array_map("myfunction",$a));
        ?>
        ```

    14. **array_column()**: This function returns the values from a single column in the input array.

        ```
        <?php
          $a = array(
            array(
              'id' => 5698,
              'first_name' => 'Peter',
              'last_name' => 'Griffin',
            ),
            array(
              'id' => 4767,
              'first_name' => 'Ben',
              'last_name' => 'Smith',
            ),
            array(
              'id' => 3809,
              'first_name' => 'Joe',
              'last_name' => 'Doe',
            )
          );

          $last_names = array_column($a, 'last_name');
          print_r($last_names);
        ?>
        ```

    **[⬆ Back to Top](#table-of-contents)**

11. ### Explain some of the PHP string functions?

    1. **strlen()**: This function returns the length of a string.

       ```
       <?php
         echo strlen("Hello World!"); //output: 12
       ?>
       ```

    2. **str_word_count()**: This function counts the number of words in a string.

       ```
       <?php
         echo str_word_count("Hello World!"); //output: 2
       ?>
       ```

    3. **strrev()**: This function reverses a string.

       ```
       <?php
         echo strrev("Hello World!"); //output: !dlroW olleH
       ?>
       ```

    4. **strpos()**: This function searches for a specific text within a string. If a match is found, the function returns the character position of the first match. If no match is found, it will return FALSE.

       ```
       <?php
         echo strpos("Hello World!", "World"); //output: 6
       ?>
       ```

    5. **str_replace()**: This function replaces some characters with some other characters in a string.

       ```
       <?php
         echo str_replace("World", "Peter", "Hello World!"); //output: Hello Peter!
       ?>
       ```

    6. **strtolower()**: This function converts a string to lowercase.

       ```
        <?php
          echo strtolower("Hello World!"); //output: hello world!
        ?>
       ```

    7. **strtoupper()**: This function converts a string to uppercase.

       ```
        <?php
          echo strtoupper("Hello World!"); //output: HELLO WORLD!
        ?>
       ```

    8. **ucfirst()**: This function converts the first character of a string to uppercase.

       ```
        <?php
          echo ucfirst("hello world!"); //output: Hello world!
        ?>
       ```

    9. **ucwords()**: This function converts the first character of each word in a string to uppercase.

       ```
        <?php
          echo ucwords("hello world!"); //output: Hello World!
        ?>
       ```

    10. **trim()**: This function removes whitespace or other predefined characters from both sides of a string.

        ```
         <?php
           echo trim(" Hello World! "); //output: Hello World!
         ?>
        ```

    11. **substr()**: This function returns a part of a string.

        ```
         <?php
           echo substr("Hello World!", 6); //output: World!
         ?>
        ```

    12. **str_repeat()**: This function repeats a string a specified number of times.

        ```
         <?php
           echo str_repeat("Hello World!", 3); //output: Hello World! Hello World! Hello World!
         ?>
        ```

    13. **explode()**: This function breaks a string into an array.

        ```
         <?php
           print_r(explode(" ", "Hello World!")); //output: Array ( [0] => Hello [1] => World! )
         ?>
        ```

    **[⬆ Back to Top](#table-of-contents)**

12. ### Differentiate between require and include?

    **require** and **include** both are used to include a file but if data is not found include sends warning and continue execution script while require sends fatal error and stops the execution.

    **Example**:

    ```
    <?php
      include ('myFile.php');
      echo "Hello World!";
    ?>

    <?php
      require ('myFile.php');
      echo "Hello World!";
    ?>

    ```

    **[⬆ Back to Top](#table-of-contents)**

13. ### Explain PHP Variables Scope?

    **PHP has three different variable scopes**:

    1. **Local** : A variable declared within a function has a LOCAL SCOPE and can only be accessed within that function.
    2. **Global** : A variable declared outside a function has a GLOBAL SCOPE and can only be accessed outside a function.
    3. **Static** : A variable declared within a function with a static keyword has a STATIC SCOPE and can be accessed within a function.

    **Example**:

    ```
       <?php
        // Global scope
        $globalVar = "I'm a global variable";

        function test()
        {
          // Local scope
          $localVar = "I'm a local variable";
          echo $localVar . "\n";

          // Access global variable inside function
          global $globalVar;
          echo $globalVar . "\n";

          // Static variable
          static $staticVar = 0;
          $staticVar++;
          echo $staticVar . "\n";

         }

         test();

        ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

14. ### Explain PHP Superglobals variables?

    **PHP Superglobals variables** are built-in variables that are always available in all scopes.

    **PHP Superglobals variables** are used to access global variables from any function, class or file.

    **PHP Superglobals variables** are as follows:

    1. **$GLOBALS** : It is used to access global variables from anywhere in the PHP script (also from within functions or methods).

    2. **$\_SERVER** : It is used to get the information about the server.

    3. **$\_REQUEST** : It is used to collect data after submitting an HTML form.

    4. **$\_POST** : It is used to collect form data after submitting an HTML form with method="post".

    5. **$\_GET** : It is used to collect form data after submitting an HTML form with method="get".

    6. **$\_FILES** : It is used to collect form data after submitting an HTML form with method="post" and enctype="multipart/form-data".

    7. **$\_ENV** : It is used to get the information about the environment.

    8. **$\_COOKIE** : It is used to get the information about the cookie.

    9. **$\_SESSION** : It is used to get the information about the session.

    **[⬆ Back to Top](#table-of-contents)**

15. ### What are the ways to define a constant in PHP?

    There are two ways to define a constant in PHP:

    1. **Using define() function** : This function is used to define a constant. It takes two parameters: the constant name and its value.

       ```
       <?php
         define("GREETING", "Welcome to W3Docs.com!");
         echo GREETING;
       ?>
       ```

    2. **Using const keyword** : This keyword is used to define a constant. It takes two parameters: the constant name and its value.

       ```
       <?php
         const GREETING = "Welcome to W3Docs.com!";
         echo GREETING;
       ?>
       ```

    **[⬆ Back to Top](#table-of-contents)**

16. ### What is autoloading in php?

    **Autoloading** is a technique that allows PHP to load classes automatically so that you don't need to include them manually. It is a more flexible alternative to \_\_autoload().

    **Example**:

    ```
    <?php
      spl_autoload_register(function ($class_name) {
        include $class_name . '.php';
      });

      $obj  = new MyClass1();
      $obj2 = new MyClass2();
      $obj3 = new MyClass3();
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

17. ## What is the difference between == and ===?

    **==** checks for equality only, whereas **===** checks for equality and type.

    **Example**:

    ```
    <?php
      $num = 5;
      $num2 = '5';

      if ($num == $num2) {
        echo 'Equal';
      } else {
        echo 'Not equal';
      }

      if ($num === $num2) {
        echo 'Equal';
      } else {
        echo 'Not equal';
      }
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

18. ## What is magic number in PHP?

    **Magic numbers** are the numeric values that are used without any explanation of what they mean or why they are used. It is considered as a bad programming practice because it makes the code hard to understand and maintain.

    **Example**:

    ```
     <?php
       function calculateArea($radius)
       {
         return 3.14 * $radius * $radius;
       }

       echo calculateArea(5);
     ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

19. ## What is htmlspecialchars in php?

    **htmlspecialchars()** function converts some predefined characters to HTML entities. It is used to avoid cross-site scripting (XSS) attacks.

    **Example**:

    ```
    <?php
      $str = "Hello World!";
      echo htmlspecialchars($str);
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

20. ## What is the use of DIR in PHP?

    **DIR** is a magic constant that returns the directory of the current file.

    **Example**:

    ```
    <?php
      echo __DIR__;
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

21. ## What is the purpose of the extract() function?

    **extract()** is an inbuilt function in PHP. The extract() function does array to variable conversion. That is it converts array keys into variable names and array values into variable value.

    **Example**:

    ```
    <?php
      $fruits = array("apple" => "red", "banana" => "yellow");
      extract($fruits);
      echo "Apple is $apple and Banana is $banana";
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

22. ## What is compact() function in PHP?

    **compact()** is an inbuilt function in PHP. The compact() function creates an array from variables and their values.

    **Example**:

    ```
    <?php
      $name = "Peter";
      $age = "41";
      $city = "New York";

      $result = compact("name", "age", "city");
      print_r($result);
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

23. ## What are the advantages of using namespaces in PHP?

    **Namespaces** are used to avoid naming collisions between classes, functions, constants, etc. It allows us to group classes, interfaces, functions, and constants into a logical group.

    **Example**:

    ```
    <?php
      namespace MyProject;

      const CONNECT_OK = 1;
      class Connection { /* ... */ }
      function connect() { /* ... */  }

    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

24. ## What does call_user_func() do in PHP?

    **call_user_func()** is an inbuilt function in PHP which is used to call the callback given by the first parameter and passes the remaining parameters as argument. It is used to call the user-defined functions.

    **Example**:

    ```
    <?php
      function hello($name)
      {
        echo "Hello $name";
      }

      call_user_func('hello', 'Peter');
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

25. ## What is the use of session in PHP?

    **Session** is used to store information about the user across the various pages of a website. It is used to store and access the user information as well as variables across the pages of a website.

    **Example**:

    ```
    <?php
      session_start();
      $_SESSION['name'] = 'Peter';
      $_SESSION['age'] = '41';
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

26. ## What are the cookies in PHP?

    **Cookies** is a small piece of information which is stored at client browser. It is used to recognize the user.
    Cookie is created at server side and saved to client browser. Each time when client sends request to the server, cookie is embedded with request. Such way, cookie can be received at the server side.

    **Example**:

    ```
    <?php
      $name = "Peter";
      $age = "41";
      setcookie($name, $age, time() + (86400 * 30), "/");
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

27. ## What does session_get_cookie_params() do in PHP?

    **session_get_cookie_params()** is an inbuilt function in PHP which is used to get the session cookie parameters.

    **Example**:

    ```
    <?php
      print_r(session_get_cookie_params());
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

28. ## What does session_regenerate_id() do in PHP?

    **session_regenerate_id()** is an inbuilt function in PHP which is used to regenerate the session ID.

    **Example**:

    ```
    <?php
      session_start();
      session_regenerate_id();
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

29. ## What is the difference between unset() and unlink()?

    **unset()** is a PHP inbuilt function, which is used to destroys the specified variables.

    **unlink()** is a PHP inbuilt function, which is used to delete a certain file.

    **Example**:

    ```
    <?php
      $name = "Peter";
      unset($name);

      $file = "test.txt";
      unlink($file);

    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

30. ## What is the difference between new self and new static in PHP?

    **new self** refers to the same class in which the new keyword is actually written.

    **new static** refers to the same class in which the new keyword is actually written at runtime.

    **Example**:

    ```
    <?php
      class A
      {
        public static function get_self()
        {
          return new self();
        }

        public static function get_static()
        {
          return new static();
        }
      }

      class B extends A
      {

      }

      echo get_class(B::get_self()); // Output: A
      echo get_class(B::get_static()); // Output: B
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

31. ## What is the exception handling in PHP?

    **Exception handling** in PHP allows you to manage errors or exceptional situations that might occur during the execution of a script.

    **PHP provides the following specialized keywords for this purpose.**

    **try** a function using an exception should be in a "try" block. If the exception does not trigger, the code will continue as normal. However if the exception triggers, an exception is "thrown".

    **throw** this is how you trigger an exception. Each "throw" must have at least one "catch"

    **catch** a "catch" block retrieves an exception and creates an object containing the exception information

    **finally** the finally block can be specified after or in place of catch block. It always executes just after the try and catch block whether an exception has been thrown or not, and before the normal execution restarts.

    **Example**:

    ```
    <?php
      function divide($dividend, $divisor) {
        if($divisor == 0) {
          throw new Exception("Division by zero");
        }
        return $dividend / $divisor;
      }

      try {
        echo divide(5, 0);
      } catch(Exception $e) {
        echo " Unable to divide. ";
      } finally {
        echo "Process complete.";
      }
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

32. ## What does HTTP_REFERER do in PHP?

    **HTTP_REFERER** is a PHP inbuilt variable which is used to return the URL of the page from which the request was sent.

    **Example**:

    ```
    <?php
      echo $_SERVER['HTTP_REFERER'];
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

33. ## What are magic methods and how to use them in PHP ?

    **Magic methods** are special methods that are called automatically when certain conditions are met. They are always preceded with two underscores.

    **Some of the magic methods are as follows:**

    **\_\_construct()** : The **construct()** method is called automatically when a class is initiated, and it has a function name **construct()**. This method can be used to initialize class properties.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        function intro() {
          echo "The fruit is {$this->name} and the color is {$this->color}.";
        }
      }

      $apple = new Fruit("Apple", "red");
      $apple->intro();
    ?>
    ```

    **\_\_destruct()** : The **destruct()** method is called automatically when the object is destroyed or the script is stopped or exited. The **destruct()** method that will be called last, after all the other methods have been called.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        function intro() {
          echo "The fruit is {$this->name} and the color is {$this->color}.";
        }

        function __destruct() {
          echo "The fruit is {$this->name} and the color is {$this->color}.";
        }
      }

      $apple = new Fruit("Apple", "red");
      $apple->intro();
    ?>
    ```

    **\_\_call()** : The **call()** method is triggered when invoking inaccessible methods in an object context. The **call()** method accepts two parameters: the first parameter ($name) contains the name of the method that was called, the second parameter ($arguments) contains an enumerated array that contains the parameters passed to the $name method.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        function intro() {
          echo "The fruit is {$this->name} and the color is {$this->color}.";
        }

        function __call($name, $arguments) {
          echo "The method $name does not exist";
        }
      }

      $apple = new Fruit("Apple", "red");
      $apple->hello();
    ?>
    ```

    **\_\_callStatic()** : The **callStatic()** method is triggered when invoking inaccessible methods in a static context. The **callStatic()** method accepts two parameters: the first parameter ($name) contains the name of the method that was called, the second parameter ($arguments) contains an enumerated array that contains the parameters passed to the $name method.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        function intro() {
          echo "The fruit is {$this->name} and the color is {$this->color}.";
        }

        public static function __callStatic($name, $arguments) {
          echo "The method $name does not exist";
        }
      }

      Fruit::hello();
    ?>
    ```

    **\_\_get()** : The **get()** method is utilized for reading data from inaccessible properties. The **get()** method accepts one parameter: the $name property name.

    **Example**:

    ```
    <?php
      class Fruit {
        private $name;

        public function __construct($name) {
          $this->name = $name;
        }

        public function __get($name) {
          return $this->$name;
        }
      }

      $apple = new Fruit('Apple');
      echo $apple->name;
    ?>
    ```

    **\_\_set()** : The **set()** method is run when writing data to inaccessible properties. The **set()** method accepts two parameters: the $name property name and the $value property value.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;

        public function __construct($name) {
          $this->name = $name;
        }

        public function __set($name, $value) {
          $this->$name = $value;
        }
      }

      $fruit = new Fruit('Apple');
      $fruit->name = 'Mango';
      echo $fruit->name;
    ?>
    ```

    **\_\_isset()** : The **isset()** method is triggered by calling isset() or empty() on inaccessible properties. The **isset()** method accepts one parameter: the $name property name.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;

        public function __construct($name) {
          $this->name = $name;
        }

        public function __isset($name) {
          return isset($this->$name);
        }
      }

      $fruit = new Fruit('Apple');
      var_dump(isset($fruit->name));
    ?>
    ```

    **\_\_unset()** : The **unset()** method is invoked when **unset()** is used on inaccessible or non-existing properties. The **unset()** method accepts one parameter: the $name property name.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;

        public function __construct($name) {
          $this->name = $name;
        }

        public function __unset($name) {
          unset($this->$name);
        }
      }

      $fruit = new Fruit('Apple');
      unset($fruit->name);
      echo $fruit->name;
    ?>
    ```

    **\_\_sleep()** : The **sleep()** method is used for cleanup tasks. This method is executed when the **serialize()** method is called. The **sleep()** method accepts no parameters and returns an array with the names of all the properties that should be saved.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __sleep() {
          return array('name', 'color');
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $data = serialize($fruit);
      echo $data;
    ?>
    ```

    **\_\_wakeup()** : The **wakeup()** method is used for reestablishing any database connections that may have been lost during serialization and perform other reinitialization tasks. This method is executed when the **unserialize()** method is called. The **wakeup()** method accepts no parameters and does not return any value.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __sleep() {
          return array('name', 'color');
        }

        public function __wakeup() {
          echo "The color of {$this->name} is {$this->color}.";
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $data = serialize($fruit);
      echo $data;
      $fruit = unserialize($data);
    ?>
    ```

    **\_\_serialize()** : The **serialize()** method is used to define a serialization-friendly arbitrary representation of the object.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __sleep() {
          return array('name', 'color');
        }

        public function __wakeup() {
          echo "The color of {$this->name} is {$this->color}.";
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $data = serialize($fruit);
      echo $data;
    ?>
    ```

    **\_\_unserialize()** : The **unserialize()** method is used to converts serialized data back into actual data.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __sleep() {
          return array('name', 'color');
        }

        public function __wakeup() {
          echo "The color of {$this->name} is {$this->color}.";
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $data = serialize($fruit);
      echo $data;
      $fruit = unserialize($data);
    ?>
    ```

    **\_\_toString()** : The **toString()** method allows a class to decide how it will react when it is treated like a string. The **toString()** method must return a string value, otherwise a fatal **E_RECOVERABLE_ERROR** type error is issued.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __toString() {
          return "The color of {$this->name} is {$this->color}.";
        }
      }

      $fruit = new Fruit('Apple', 'red');
      echo $fruit;
    ?>
    ```

    **\_\_invoke()** : The **invoke()** method is called when a script tries to call an object as a function. The **invoke()** method accepts arguments as an array, and these arguments are the arguments passed to the object when it was called.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __invoke() {
          echo "The color of {$this->name} is {$this->color}.";
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $fruit();
    ?>
    ```

    **\_\_set_state()** : The **set_state()** method is called when var_export() is called on an object. The **set_state()** method accepts an array of properties exported by var_export().

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public static function __set_state($an_array) {
          $obj = new Fruit($an_array['name'], $an_array['color']);
          return $obj;
        }
      }

      $fruit = new Fruit('Apple', 'red');
      eval('$b = ' . var_export($fruit, true) . ';');
      var_dump($b);
    ?>
    ```

    **\_\_clone()** : The **clone()** method is called when an object is cloned. The **clone()** method can be used to modify the properties of the cloned object before it is used.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __clone() {
          $this->color = 'yellow';
        }
      }

      $fruit = new Fruit('Apple', 'red');
      $fruit2 = clone $fruit;
      echo $fruit->color;
      echo $fruit2->color;
    ?>
    ```

    **\_\_debugInfo()** : The **debugInfo()** method is called by **var_dump()** when dumping an object to get the properties that should be shown. If the **debugInfo()** method is not defined, then all public, protected, and private properties will be shown.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }

        public function __debugInfo() {
          return [
            'name' => $this->name,
            'color' => $this->color,
          ];
        }
      }

      $fruit = new Fruit('Apple', 'red');
      var_dump($fruit);
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

34. ## What is ReflectionClass class in PHP?

    **ReflectionClass** class is used to get information about a class.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }
      }

      $reflection = new ReflectionClass('Fruit');
      var_dump($reflection);
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

35. ## What is ReflectionMethod class in PHP?

    **ReflectionMethod** class is used to get information about a method.

    **Example**:

    ```
    <?php
      class Fruit {
        public $name;
        public $color;

        public function __construct($name, $color) {
          $this->name = $name;
          $this->color = $color;
        }
      }

      $reflection = new ReflectionMethod('Fruit', '__construct');
      var_dump($reflection);
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

36. ## What is the use of sscanf in PHP?

    **sscanf()** is an inbuilt function in PHP which is used to read formatted input from a string. It is used to parse a string from left to right using a specified format.

    **Example**:

    ```
    <?php
      $str = "Peter is 41 years old.";
      sscanf($str, "%s is %d years old.", $name, $age);
      echo $name . " " . $age;
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**

37. ## What does list() do in PHP?

    **list()** is an inbuilt function in PHP which is used to assign values to a list of variables in one operation.

    **Example**:

    ```
    <?php
      $fruits = array("apple", "banana", "cherry");
      list($a, $b, $c) = $fruits;
      echo $a . " " . $b . " " . $c;
    ?>
    ```

    **[⬆ Back to Top](#table-of-contents)**
