# 🪱 Split and Strip in Python

'split()' is a method that is used to split a string into a list of substrings based on a specified separator. By default, the separator is any whitespace character, such as a space or a tab. Here is an example of how to use the 'split()' method in Python.

```python
string = "Hello, world!"
mylist = string.split(",")
print(mylist)
```

In the example, we define a string 'string' and use the 'split()' method to split into a list of substrings based on the comma separator. The resulting list is '\['Hello', ' world!']'.

'strip()' is a method that is used to remove leading and trailing whitespace characters from a string.

```python
string = " Hello, world!"
new_string = string.strip()
print(new_string)
```

In this example, we define a string 'string' with leading and trailing whitespace characters and use the 'strip()' method to remove them. The resulting string is '"Hello, world!"'.
