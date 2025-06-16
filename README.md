# my-python-tool
## Overview

Python is a flexible and powerful programming language increasingly used in development research for data cleaning, analysis, visualization, and reproducible workflows. While Stata and R are commonly used in DIME, Python is ideal for data pipelines, API access, automation, and integrating with machine learning and natural language processing tools.

## Installation

First, you can check if Python is already installed on your computer. To do this open your terminal (Command Prompt or Terminal) and type:
 <code>python --version</code>
or 
 <code>python3 --version</code>

Otherwise you can install python using this [beginners guide](https://wiki.python.org/moin/BeginnersGuide/Download/).

## Creating a Virtual Environment

Always create a virtual environment for each project to isolate dependencies and improve reproducibility.

*Create a new environment:

<code>python -m venv venv</code>

*Activate the environment (Windows):

<code>venv\Scripts\activate</code>

*Activate the environment (macOS/Linux):

<code>source venv/bin/activate</code>

Once activated, you can install project-specific packages without affecting your global Python setup.


## Installing Packages

Use <code>pip</code> to install packages, and document them in a requirements.txt file:

```python
pip install pandas numpy matplotlib jupyter
pip freeze > requirements.txt
```

 
Or use <code>conda</code> if you're managing environments with Anaconda/Miniconda:

```python
conda create --name myenv python=3.10
conda activate myenv
conda install pandas numpy matplotlib jupyter
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


## Loops in Python

Loops are often used in automation, batch operations, and simulations. Use them responsibly—Python is slower than R or Stata for large, row-wise operations.

##<code>for</code> loop
```python
for i in range(5):
    print(i)
```
##Looping Through Lists 
```python
names = ['Alice', 'Bob', 'Ceren']
for name in names:
    print(f"Hello {name}")
```

## Web Scraping 

Web scraping means to extract and arrange data from a web page. [Here](https://github.com/worldbank/dime-python-training/blob/main/I%20-%20Introduction/archive/web%20scraping%20example/Web-scraping%20basic%20example.ipynb) you can find a basic example for web scraping. For the training session recording, please refer to the related trainings. 

## Related DIME Analytics Trainings

* [Intro to Python](https://osf.io/8sgrh/files/osfstorage/5fd2f84c0694b7013af371fd/)
* [Introduction to Python and Web Scraping](https://osf.io/8sgrh/files/osfstorage/6040d32267386c040561d343/)
* [Intro to APIs](https://osf.io/8sgrh/files/osfstorage/605c0b5dfbc498004a402ff7/)
