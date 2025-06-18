# my-python-tool
## Overview

Python is a flexible and powerful programming language increasingly used in development research for data cleaning, analysis, visualization, and reproducible workflows. While Stata and R are commonly used in development research, Python is ideal for data pipelines, API access, automation, and integrating with machine learning and natural language processing tools.

## Installation

First, you can check if Python is already installed on your computer. To do this open your terminal (Command Prompt or Terminal) and type:
 <code>python --version</code>
or 
 <code>python3 --version</code>

Otherwise you can install python using this [beginners guide](https://wiki.python.org/moin/BeginnersGuide/Download/).

## Creating a Virtual Environment

Always create a virtual environment for each project to isolate dependencies and improve reproducibility.

* Create a new environment:

<code>python -m venv venv</code>

* Activate the environment (Windows):

<code>venv\Scripts\activate</code>

* Activate the environment (macOS/Linux):

<code>source venv/bin/activate</code>

Once activated, you can install project-specific packages without affecting your global Python setup.


## Installing Packages

Use <code>pip</code> on your Command Prompt to install packages, and document them in a requirements.txt file:

```python
pip install pandas numpy matplotlib jupyter
pip freeze > requirements.txt
```


## Data Types

Understanding data types is key to avoiding bugs in analysis and loops. Keep in mind that Python has thousands of different data types. These are some basic examples:

| Type       | Example         | Description               |
| ---------- | --------------- | ------------------------- |
| `int`      | `x = 5`         | Integer                   |
| `float`    | `x = 5.2`       | Decimal number            |
| `str`      | `x = "text"`    | String (text)             |
| `bool`     | `x = True`      | Boolean (`True`, `False`) |
| `list`     | `x = [1, 2, 3]` | Ordered collection        |
| `dict`     | `x = {"a": 1}`  | Key-value pairs           |
| `NoneType` | `x = None`      | Null equivalent           |

Use `type(x)` to check the data type of a variable.

You can assign values to variables and do mathematical calculations, the variables you create will be available in memory until you restart Python or explicitly delete it.
For example:

```python
x = 10 
y = 5 
z = 10 + 5 
z    # This will return 15
```

Most common mathematical operations are listed below:

| Operation             | Symbol / Function | Example        | Result |
| --------------------- | ----------------- | -------------- | ------ |
| Addition              | `+`               | `3 + 2`        | `5`    |
| Subtraction           | `-`               | `7 - 4`        | `3`    |
| Multiplication        | `*`               | `6 * 3`        | `18`   |
| Division (float)      | `/`               | `7 / 2`        | `3.5`  |
| Division (floor)      | `//`              | `7 // 2`       | `3`    |
| Modulo (remainder)    | `%`               | `7 % 2`        | `1`    |
| Power of              | `**`              | `2 ** 3`       | `8`    |
| Absolute value        | `abs()`           | `abs(-7)`      | `7`    |
| Round to whole number | `round()`         | `round(3.6)`   | `4`    |
| Max value             | `max()`           | `max(2, 5, 1)` | `5`    |
| Min value             | `min()`           | `min(2, 5, 1)` | `1`    |

## Methods 

A method is a function that is associated with an object. You call it on the object, and it can use or modify that object’s data. In simple terms, a method is just a function that's tied to a specific data type or object.
For example:
```python
object.method(arguments)
```
String method:
```python
country = "spain"
print(name.upper())
```
<code>upper()</code> is a string method. It returns <code>"SPAIN"</code>, the uppercase version of our string. However, it does not change <code>country</code> if you don't assign the result of your function. 



## Loops in Python

Loops are often used in automation, batch operations, and simulations.

### <code>for</code> loop
```python
for i in range(5):
    print(i)
```
### Looping Through Lists 
```python
names = ['Alice', 'Bob', 'Ceren']
for name in names:
    print(f"Hello {name}")
```

## Web Scraping 

Web scraping means to extract and arrange data from a web page. [Here](https://github.com/worldbank/dime-python-training/blob/main/I%20-%20Introduction/archive/web%20scraping%20example/Web-scraping%20basic%20example.ipynb) you can find a basic example for web scraping. For the training session recording, please refer to the related trainings. 

## Additional Resources 
* World Bank Development Economics' [Python course](https://github.com/worldbank/dec-python-course) material

## Related DIME Analytics Trainings

* [Intro to Python](https://osf.io/8sgrh/files/osfstorage/5fd2f84c0694b7013af371fd/)
* [Introduction to Python and Web Scraping](https://osf.io/8sgrh/files/osfstorage/6040d32267386c040561d343/)
* [Data processing in Python using Pandas](https://osf.io/yw5vs)
* [Data pipelines in Python](https://osf.io/gt7dm)
