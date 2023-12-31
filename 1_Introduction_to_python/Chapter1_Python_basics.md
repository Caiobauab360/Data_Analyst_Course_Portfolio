# Introduction to python course

**Course description:**

Python is a general-purpose programming language that is becoming ever more popular for data science. Companies worldwide are using Python to harvest insights from their data and gain a competitive edge. Unlike other Python tutorials, this course focuses on Python specifically for data science. In our Introduction to Python course, you’ll learn about powerful ways to store and manipulate data, and helpful data science tools to begin conducting your own analyses. Start DataCamp’s online Python curriculum now.

# Python Basics

An introduction to the basic concepts of Python. Learn how to use Python interactively and by using a script. Create your first variables and acquaint yourself with Python's basic data types.

**Personal notes:**

Required Knowledge:

-Python

-Database

-English

Basic Mathematical Functions:

-Addition: +

-Subtraction: -

-Multiplication: *

-Division: /

-Exponentiation: **

-Modulo (Remainder of division): %

-Square Root: ** and then use /

**Exercices:**

**When to use Python?**
Python is a flexible language. For which applications can you use Python?
    
    For quick calculations, develop a database-driven website, clean and analyze data.

**The Python Interface**
Hit Run Code to run your first Python code with Datacamp and see the output!

Notice the script.py window; this is where you can type Python code to solve exercises. You can hit Run Code and Submit Answer as often as you want. If you're stuck, you can click Get Hint, and ultimately Get Solution.

You can also use the IPython Shell interactively by typing commands and hitting Enter. Here, your code will not be checked for correctness so it is a great way to experiment.
-Experiment in the IPython Shell; type 5 / 8, for example.
-Add another line of code to script.py, print(7 + 10), to be checked for correctness.
-Hit Submit Answer to execute the Python script and receive feedback.
        
        # Example, do not modify!
        print(5 / 8)

        # Print the sum of 7 and 10
        print(17)

**Any comments?**
You can also add comments to your Python scripts. Comments are important to make sure that you and others can understand what your code is about and do not run as Python code.

They start with # tag. See the comment in the editor, # Division; now it's your turn to add a comment!
       
        # Division
        print(5 / 8)
        # Addition
        print(7 + 10)   

**Python as a calculator**
Python is perfectly suited to do basic calculations. It can do addition, subtraction, multiplication and division.

The code in the script gives some examples.

Now it's your turn to practice!
-Print the sum of 4 + 5.
-Print the result of subtracting 5 from 5.
-Multiply 3 by 5.
-Divide 10 by 2.

        # Addition, subtraction
        print(5 + 5)
        print(5 - 5)
        
        # Multiplication, division, modulo, and exponentiation
        print(3 * 5)
        print(10 / 2)
        print(18 % 7)
        print(4 ** 2)

        # Calculate two to the power of five
        print(2**5)

# Variables and Types

Learn to store, access, and manipulate data in lists: the first step toward efficiently working with huge amounts of data.

**Personal notes:**

Types of Variables:

-Integers: int

-Real Numbers: float

-String (str) (for text inputs): ' ' or " "

-Boolean (bool): can be true or false

**Exercices:** 

**Variable Assignment**

In Python, a variable allows you to refer to a value with a name. To create a variable x with a value of 5, you use =, like this example:

x = 5
You can now use the name of this variable, x, instead of the actual value, 5.

Remember, = in Python means assignment, it doesn't test equality!

-Create a variable savings with the value of 100.

-Check out this variable by typing print(savings) in the script.

        # Create a variable savings
        savings = 100
        print(savings)
        # Print out savings

**Other variable types**

In the previous exercise, you worked with the integer Python data type:

int, or integer: a number without a fractional part. savings, with the value 100, is an example of an integer.
Next to numerical data types, there are three other very common data types:

float, or floating point: a number that has both an integer and fractional part, separated by a point. 1.1, is an example of a float.
str, or string: a type to represent text. You can use single or double quotes to build a string.
bool, or boolean: a type to represent logical values. It can only be True or False (the capitalization is important!).

-Create a new float, half, with the value 0.5.

-Create a new string, intro, with the value "Hello! How are you?".

-Create a new boolean, is_good, with the value True.
        # Create a variable desc
        desc = "compound interest"

        # Create a variable profitable
        profitable = True

**Guess the type**
To find out the type of a value or a variable that refers to that value, you can use the type() function. Suppose you've defined a variable a, but you forgot the type of this variable. To determine the type of a, simply execute:

type(a)
We already went ahead and created three variables: a, b and c. You can use the IPython shell to discover their type. Which of the following options is correct?

        a is of type float, b is of type str, c is of type bool.

**Operations with other types**

Hugo mentioned that different types behave differently in Python.

When you sum two strings, for example, you'll get different behavior than when you sum two integers or two booleans.

In the script some variables with different types have already been created. It's up to you to use them.

-Calculate the product of monthly_savings and num_months. Store the result in year_savings.

-What do you think the resulting type will be? Find out by printing out the type of year_savings.

-Calculate the sum of intro and intro and store the result in a new variable doubleintro.

-Print out doubleintro. Did you expect this?

    savings = 100
    growth_multiplier = 1.1
    desc = "compound interest"

    # Assign product of savings and growth_multiplier to year1
    year1 = savings*growth_multiplier*1

    # Print the type of year1
    print(type(year1))

    # Assign sum of desc and desc to doubledesc
    doubledesc = desc + desc

    # Print out doubledesc
    print(doubledesc)

**Type conversion**

Using the + operator to paste together two strings can be very useful in building custom messages.

Suppose, for example, that you've calculated your savings want to summarize the results in a string.

To do this, you'll need to explicitly convert the types of your variables. More specifically, you'll need str(), to convert a value into a string. str(savings), for example, will convert the integer savings to a string.

Similar functions such as int(), float() and bool() will help you convert Python values into any type.

-Hit Run Code to run the code. Try to understand the error message.

-Fix the code such that the printout runs without errors; use the function str() to convert the variables savings and total_savings to strings.

-Convert the variable pi_string to a float and store this float as a new variable, pi_float.
    # Definition of savings and result
    savings = 100
    result = 100 * 1.10 ** 7

    # Fix the printout
    print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

    # Definition of pi_string
    pi_string = "3.1415926"

    # Convert pi_string into float: pi_float
    pi_float = float(pi_string)

**Can Python handle everything?**

Now that you know something more about combining different sources of information, have a look at the four Python expressions below. Which one of these will throw an error? You can always copy and paste this code in the IPython Shell to find out!

    "The correct answer to this multiple choice exercise is answer number" + 2. 