# Introduction to Python

## Reading

Computing Skills for Biologists, Chapter 3 (Basic Programming), pgs. 81-119

## What is Python?

- Interpreted, high-level language
- Very popular among computational biologists
- One of the most "human readable" programming languages
- One of the few languages where line indentation is actually interpreted as part of the code
- Python is _much_ less picky than bash about spacing within lines, though
- Dynamically typed (don't worry, we'll get to this later)

## Three Ways to Run Python

### Python Interpreter

- Unlike many programming languages (e.g., C++ and Java), Python can be executed interactively.
- To start the Python interpreter, simply open up a Terminal window and type `python`.
- Once the Python prompt (`>>>`) appears, type:
    - `a = 3`
    - `print(a)`
- What do you see?
- To exit the Python interpreter, type `quit()`.

### Command-line Python

- Now, put those same commands in a text file ending with a `.py` extension (e.g., `test.py`).
- At the bash command prompt, type `python test.py`.
- What do you see?
- The `.py` extension isn't required, but is conventional for Python code.

### Jupyter Notebooks

- Jupyter notebooks are a special type of file that allows formatted notes to be mixed with Python code.
- These notebooks can be run on smic through OnDemand.
- To open a Jupyter notebook, go to the "Interactive Apps" menu at the top and select "Jupyter Notebook".

## Basic Python Data Types

- Numbers
    - Note that, unlike bash, Python can handle _both_ integers and floating point (decimal) numbers.
    - Integers - `myInt = 10`
    - Floating point numbers (decimals) - `myFloat = 3.21312`
    - If running Python interactively, variable values can be seen just by typing the name of the variable - `myFloat`.
    - If running Python in a script, variable values can be printed by using the `print()` funtion - `print(myFloat)`.
    - Changing numbers from one type to another is one form of "type casting".

- Strings - `myStr = "This is a string."`
    - Strings can be of any length, but are always defined with quotes.
    - Individual characters, or subsets of characters, can be accessed using square brackets - []
      - String indices (and all indices in Python) start at 0
      - `myStr = "biology"`
      - `myStr[0]`
      - A range of indices can be defined with a colon
      - `myStr[2:5]`
    - Strings can be concatenated together with the `+` operator.
      - `myStr = "biology"`
      - `newString = myStr + "_is_super_interesting"`
      - `newString`

- Booleans - `True` or `False`
    - These variables can take the values `True` or `False` only.
      - `myBool = True`
    - These are the data types used in things like `if...else` statements and `while` loops.
    - Logical statements, like `myNum > 3` or `myStr == "test"`, return a boolean variable indicating the result of the comparison
    - In Python, the value of a Boolean can be reversed by preceding it with `not`.

## Functions

- Functions are the verbs of a programming language
- Functions take some variables or objects as input (arguments) and either do something with them or return a new variable/object.
- Functions are always written like this - `myFunction(object1,object2,...)`
- They _always_ have parentheses, even if they don't need any arguments to be passed to them
    - For example, `myFunction()`
- The number and type of arguments needed is specific to each function
- Perhaps the simplest function to use is `print()`. `print()` can take an arbitrary number of variables as arguments and will print them to the screen.
- Here are a few other really useful functions and what they do:
    - `len(string)` - Takes one argument (a string) and returns its length
    - `abs(number)` - Takes one argument (either an integer or a float) and returns its absolute value
    - `round(float)` - Takes one floating point number as an argument and rounds it to the nearest integer
    - `type(variable)` - Takes one variable as an argument and returns its type

## Methods
  
- Methods are functions (sort of like actions or verbs) that belong to a variable
- Methods are accessed and used by appending them to the name of a variable, separated by a `.`
- For instance, let's say we define a string - `myStr = "biOLogy  "`. Here are some really useful methods that can be used with that string:
    - `myStr.upper()` - Converts all characters in the string to uppercase
    - `myStr.lower()` - Converts all characters in the string to lowercase
    - `myStr.strip()` - Removes whitespace from the beginning or ending of the string
    - Methods can also be chained! - `myStr.strip().lower()`
    - `myStr.replace("y","ical")` - This method functions like find and replace, where the first argument is the text to find and the second argument is the text to use when replacing.
    - `myStr.split("O")` - Breaks up the string, using the character provided as an argument as the delimiter. This method then returns a list of new strings. We'll talk more about lists later.

## Comments in Python

- Just like with bash, comments are essential in Python.
- Comments are included in Python by putting a `#` at the beginning of a line.
- Many text editors have a shortcut keystroke to toggle lines between being commented and uncommented. 
- `# This is an example of a comment`

## String Formatting
  
- Python has a special way to format strings so that the values of variables can be included
- The operator `%` is used to indicate that the values of certain variables should be used to fill in a string
- The parts of the string where the values should go is indicated with placeholders (kinda like wildcards)
- The three most basic placeholders are:
    - `%d` - An integer
    - `%f` - A floating point number (i.e., a decimal)
    - `%s` - A string
- Try this:
    - `faveInt = 7`
    - `faveFloat = 3.14`
    - `faveString = phyleaux`
    - `print("Favorite integer is %d, favorite float is %f, and favorite string is %s." % (faveInt,faveFloat,faveString))`
- Note how the variables holding the values are provided in the same order inside parentheses after the `%`.

## Additional Python Resources

- [Python](https://www.python.org)
- [Software Carpentry - Intro. to Python](http://swcarpentry.github.io/python-novice-inflammation/)
- [Updated notes on Python string formatting](https://realpython.com/python-string-formatting/#2-new-style-string-formatting-strformat)
