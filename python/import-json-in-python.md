---
description: json = JavaScript Object Notation
---

# 🐍 import json in Python

In Python, `import json` is a statement that allows you to work with JSON (JavaScript Object Notation) data. JSON is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate[1](https://www.simplilearn.com/tutorials/python-tutorial/json-python)[2](https://realpython.com/lessons/what-is-json/).Python has a built-in package called `json` that provides methods for encoding and decoding JSON data. The `json` package can be used to convert JSON data to Python objects and vice versa.

```python
import json

# Open the JSON file
with open('data.json') as f:
    # Load the JSON data into a Python dictionary
    data = json.load(f)

# Access the data as a Python object
print(data['name'])
print(data['age'])
```

In this example, the `json.load()` method is used to read the JSON data from the file `data.json` and convert it into a Python dictionary. The `with` statement is used to open the file and automatically close it when the block is exited. The data can then be accessed as a Python object using the keys of the dictionary.
