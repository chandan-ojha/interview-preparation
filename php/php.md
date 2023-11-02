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
