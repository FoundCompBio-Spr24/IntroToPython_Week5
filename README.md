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
