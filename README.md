[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15345981&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1.  Python Basics:

    - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
      > ## ANSWER:
      >
      > Python is a high-level, interpreted programming language known for its simplicity, readability, and versatility. It emphasizes code readability and allows developers to express concepts in fewer lines of code compared to other languages.
      >
      > ### Key Features:
      >
      > - **Easy to Learn**: Python's syntax is designed to be intuitive and its high-level data structures make it simple to use.
      > - **Versatile**: Python is widely used in various domains such as web development, scientific computing, data analysis, artificial intelligence, and more.
      > - **Interpreted**: Python code is executed line by line, making debugging easier and facilitating rapid development.
      > - **Community and Ecosystem**: Python has a large and active community, contributing to a rich ecosystem of third-party libraries and frameworks.
      > - **Large Standard Library**: Python comes with a large collection of standard libraries that provide functionalities for tasks like regular expressions, file manipulation, and data parsing.
      >
      > ### Use Cases:
      >
      > <ol>
      > <li>Game development</li>
      > <li>Web development</li>
      > <li>Data science</li>
      > <li>GUI applications for desktops</li>
      > <li>Machine learning</li>
      > <li>Automation</li>
      > <li>Backend services</li>
      > <li>Scientific computing</li>
      > </ol>

2.  Installing Python:

    - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
      > ## ANSWER
      >
      > ## Installation of Python on Linux Kubuntu 24.04:
      >
      > - Update Package Index: Open a terminal and update the package index to ensure you have the latest information about available packages using below command:
      >
      >   `sudo apt update`
      >
      > - Install Python: By default, Ubuntu 20.04 comes with Python 3 pre-installed. You can check the version installed by typing:
      >
      >   `python3 --version`
      >
      >   If it's not installed, you can install it with:
      >
      >   `sudo apt install python3`
      >
      > - Verify if python is installed by running again the command `python3 --version`
      > - Install pip (Python Package Installer): pip is a package manager for Python that allows you to install and manage additional packages that are not included in the Python standard library. To install pip for Python 3, run:
      >
      >   `sudo apt install python3-pip`
      >
      > - Verify PIP installation by running the command:
      >
      >   `pip3 --version`
      >
      > ## Virtual Environment Setup:
      >
      > - **Install venv module (if not already installed)**:Python 3 comes with a built-in module called venv for creating virtual environments. Ensure it’s installed by running:
      >
      >   `sudo apt install python3-venv`
      >
      > - **Create a Virtual Environment**: Choose a directory where you want to create the virtual environment. For example, to create a virtual environment named myenv in your home directory (~/), run command below:
      >
      >   `python3 -m venv ~/myenv`
      >
      >   This command creates a virtual environment named myenv in the ~/ (home) directory.
      >
      > - Activate virtual environment using `source ~/myenv/bin/activate`
      > - Deactivate it using `deactivate`

3.  Python Syntax and Semantics:

    - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
      > ## ANSWER:
      >
      > `print("Hello, World!")`

4.  Data Types and Variables:

    - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
      > ## ANSWER:
      >
      > - Integer, example `x = 10`
      > - Float, example `pi = 3.14`
      > - Boolean, example `is_signed = False`
      > - String, example `my_name = "John"`
      > - List, example `even_numbers = [2, 14, 32]`
      > - Tuple, example `prime_numbers = (3, 7, 11)`
      > - Set, example `countries = {"Tanzania", "Kenya", "Uganda"}`
      > - Dictionary, example `animal = {'name' : 'Dog', 'legs' : 4}`

5.  Control Structures:

    - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

      > ## Conditional Statement (if-else):
      >
      > Conditional statements in Python allow you to execute certain blocks of code based on whether a specific condition evaluates to True or False.
      >
      > ### Syntax:

            if condition:
               # Code to execute if condition is True
            else:
               # Code to execute if condition is False

      > ### Example:

            # Checking if number is greater than 10

            number = 21

            if number > 10:
               print('The number is greater than 10')
            else:
               print('The number is not greater than 10')

      > ## Loops (for):
      >
      > Loops in Python allow you to iterate over a sequence of items (such as a list, tuple, or string) or perform a certain action repeatedly until a condition is met.
      >
      > ### Syntax:

            for item in iterable:
               # Code to execute for each item in iterable

      > ### Example

            # Iterate over a list of items and print single item

            languages = ["Kiswahili", "English", "French"]

            for language in languages:
               print(language)

6.  Functions in Python:

    - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

      > - In Python, a function is a named block of code that performs a specific task or calculates a value. Functions are defined using the `def` keyword, followed by a name for the function, parentheses `()`, and optionally parameters (arguments) enclosed in these parentheses.
      > - Functions are essential in programming because they allow for code reuse, organization, and abstraction of complex tasks into manageable units.
      >
      > ### Below is a function that takes two argumets and returns their sum:

            # A function to return sum of two numbers

            def sum_numbers(first_number, second_number):
               sum = int(first_number) + int(second_number)
               return sum

      > ### Usage:

            # Provide two numbers

            first = 22
            second = 10
            result = sum_numbers(first, second)
            print(f"The sum of {first} and {second} is {result}")

7.  Lists and Dictionaries:

    - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
      > Lists and dictionaries are both fundamental data structures in Python, but they serve different purposes and have distinct characteristics. Here are the key differences between lists and dictionaries
      >
      > ## Differences between Lists and Dictionaries:
      >
      > **Lists**
      >
      > - Lists are ordered collections of items
      > - The order of elements in a list is preserved and maintained
      > - Elements in a list are accessed using integer indices starting from 0
      > - Lists are mutable, meaning you can modify their elements after creation
      > - You can add, remove, or modify elements within a list
      > - Lists are created using square brackets `[]`
      > - Example `list = [100, "John", False, [1, 2]]`
      >
      > ## **Dictionaries**
      >
      > - Dictionaries are unordered collections of key-value pairs
      > - The order of elements in a dictionary is not guaranteed and may vary
      > - Elements (values) in a dictionary are accessed using keys rather than indices
      > - Dictionaries are mutable, so you can add, remove, or modify key-value pairs after creation
      > - Dictionaries are created using curly braces `{}` with `key: value` pairs separated by commas.
      > - Example: `country = {'name': 'Tanzania', 'population': 60000000}`

8.  Exception Handling:

    - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

      > Exception handling in Python is a mechanism that allows you to handle and respond to errors (exceptions) that occur during the execution of a program. Exceptions are runtime errors that disrupt the normal flow of a program when they are not handled properly. Python provides a structured way to manage these exceptions using `try, except, else, and finally ` blocks.
      >
      > ## Syntax:

            # Syntax of exception handling in Python

            try:
               # Code that may raise an exception
            except ExceptionType1 as e1:
               # Handle ExceptionType1
            except ExceptionType2 as e2:
               # Handle ExceptionType2
            finnaly:
               # Cleanup code or actions that should always execute

      > ## Example:

            # Example of script to handle exceptions
            # Function to devide sum of marks by the number of subjects

            try:
               marks = int(input("Enter sum of marks: "))
               subjects = int(input("Enter number of subjects: "))
               average = marks / subjects
               print(f"The avarage is {average}")
            except ValueError:
               print("Please enter valie integers")
            except ZeroDivisionError:
               print("Division by zero not allowed")
            finnaly:
               print("Division completed. Exiting the program")

9.  Modules and Packages:

    - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
      > In Python, modules and packages are key concepts for organizing and reusing code.
      >
      > - A **module** is a single Python file that contains variables, functions, and classes related to a specific functionality or purpose. It allows you to structure your code logically, making it easier to manage and maintain. Modules are imported into other Python scripts using the `import` statement, enabling you to access their contents and use them in your current program.
      >   A **package** is a collection of related modules grouped together in a directory. It includes an `__init__.py` file to indicate that the directory should be treated as a package. Packages provide a hierarchical structure to organize modules into sub-packages, facilitating modular design and large-scale application development.
      >
      > To import and use a module in your Python script, you can use `import` statement as follows:
      >
      > ### Syntax:
      >
      > `import module_name`
      >
      > ### Example:
            import math
            print(math.sqrt(49)) # prints 7

10. File I/O:

    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

      > ## Reading from a file:
      >
      > Use `open()` function with a read mode `r`
      >
      > Example `file = open('file_name.txt', 'r')`
      >
      > To read the content use either `read()`, `readline()`, `or readlines()`
      >
      > Example `content = file.read()`
      >
      > Dont forget to close the file to release system resources with `file.close()`
      >
      > ## Writing to a file:
      >
      > Use `open()` function with a write mode `w`
      >
      > Example `file = open('file_name.txt', 'w')`
      >
      > To write use `write()` function
      >
      > Example:

               file.write("This is the first line\n")
               file.write("This is the second line")

      > Always close the file with `file.close()`

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
