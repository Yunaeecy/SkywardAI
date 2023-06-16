# 🐍 Getter and Setter in Python

Basically, the main purposes of using getter and setters in object-oriented programs is to ensure data encapsulation. Private variables in Python are not actually hidden fields like in other object-oriented languages. Getters and Setters in Python are often used when:

&#x20;We use getters and setters to add validation logic around getting and setting a value.

To avoid direct access of a class field i.e., **private variables cannot be accessed directly** or modified by external user.

## Using normal function to achieve getters and setters behavior

To achieve getters and setters property, if we define normal get() and set() methods it will not reflect any special implementation.&#x20;

```python
# Python program showing a use 
# of get() and set() method in
# normal function
class Geek:
    def __init__(self, age = 0):
        self._age = age
        
    # getter method
    def get_age(self):
        return self._age
        
    # setter method
    def set_age(self, x):
        self._age = x
raj = Geek()

# setting the age using setter
raj.set_age(21)

# retrieving age using getter
print(raj.get_age())

print(raj._age)
```

A **getter method** is used to retrieve the value of an attribute or property of an object. It is typically used to provide **read-only access to an attribute**, meaning that **the value of the attribute cannot be changed directly**. Getter methods are defined using the `@property` decorator in Python.

A **setter method**, on the other hand, is used to **change the value of an attribute** or property of an object[1](https://stackoverflow.com/questions/2627002/whats-the-pythonic-way-to-use-getters-and-setters)[2](https://www.geeksforgeeks.org/getter-and-setter-in-python/)[3](https://realpython.com/python-getter-setter/)[4](https://python-reference.readthedocs.io/en/latest/docs/property/setter.html)[5](https://www.tutorialspoint.com/getter-and-setter-in-python). It is typically used to provide write-only access to an attribute, meaning that the value of the attribute **can be changed but not read.** Setter methods are defined using the `@<attribute>.setter` decorator in Python.

