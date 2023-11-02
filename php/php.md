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
| 6   | [Explain the different types of errors in PHP!](#explain-the-different-types-of-errors-in-php)                                                      |

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

    **print_r** displays information about a variable in a way that's readable by humans. **print_r** is used to print human-readable information about a variable, while **var_dump** is used to dump information about a variable that's more targeted towards developers.

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
