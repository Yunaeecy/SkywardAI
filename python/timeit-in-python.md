# 🐍 Timeit in Python

Just save the time before and after the execution of code and subtract them! But this method is not precise as there might be a background process momentarily running which disrupts the code execution and you will get significant variations in the running time of small code snippets. Timeit runs your snippet of code millions of times (default value is 1000000) so that you get the statistically most relevant measurement of code execution time! Timeit is pretty simple to use and has a command-line interface as well as a callable one.

````python
```python
import timeit


# Write the setup code
setup_code = """"
name = "Pylenin"
result_list = []
"""

# Write your main code
main_code = """"
for char in name:
    result_list.append(char)
"""

# Call the timeit function
print(timeit.timeit(stmt=main_code,
        setup=setup_code,
        number=10000))

```
````

