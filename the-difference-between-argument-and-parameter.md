# 🍒 The difference between argument and parameter

Arguments and parameters are two terms that are often used interchangeably, but they have different meanings in programming. Here are the differences between argument and parameter:

* Parameter: A parameter is a variable in a function definition that acts as a placeholder for a value that will be passed to the function when it is called. It is a part of the function's signature and defines the type and number of values that the function expects to receive.
* Argument: An argument is a value that is passed to a function when it is called. It is the actual value that is assigned to the parameter of the function. Arguments are passed to a function in the order that the parameters are defined.

In summary, a **parameter** is a variable that is **defined in a function**, while an <mark style="color:red;">**argument**</mark> is the value that is <mark style="color:red;">**passed to that parameter when the function is called**</mark>.

## "def display\_results(self) -> None:" and "def display\_results(self):"

the former specifies <mark style="color:purple;">**the return type**</mark> of the function, while the latter does not. **The "-> None"** in the first example indicates that the function <mark style="color:green;">**does not return anything.**</mark>

## Difference between "list" and "dictionary"

A <mark style="color:red;">**list\[]**</mark> is an _**ordered**_ collection of elements, and each element can be accessed using its index. A <mark style="color:red;">**dictionary{}**</mark>, on the other hand, is an _**unordered**_ collection of key-value pairs, and each value can be accessed using its key.

## print(title\[:-1]).     \[-1] in python

In Python, "print(title\[:-1])" means to print the "title" string without its last character.&#x20;

The **square brackets\[]** are used to <mark style="color:blue;">slice the string,</mark> and the <mark style="color:red;">**colon:**</mark> inside the brackets indicates that we want to slice the string. The ":-1" part of the code specifies the range of the slice, where the first colon indicates the start of the slice, and the "-1" indicates the end of the slice. In Python, <mark style="color:green;">**negative indices**</mark> are used to <mark style="color:orange;">count from the end of the string,</mark> so "-1" refers to the last character of the string. Therefore, _**"title\[:-1]" returns a new string that contains all the characters of the "title" string except for the last one.**_ Finally, the "print()" function is used to display the resulting string on the console.

## print(k,end="") and print(k,end="{:>12}".format(""))

By default, the "end" parameter is set to <mark style="color:purple;">**"\n"**</mark>, which means that <mark style="color:purple;">a newline</mark> character is printed at the end of the output. However, by setting the <mark style="color:purple;">"end" parameter to an empty string</mark>, we can print the output <mark style="color:purple;">without a newline</mark> character.

The "{:>12}" part of the code is a <mark style="color:purple;">string formatting</mark> expression that specifies how the spaces should be formatted. The <mark style="color:purple;">">" character</mark> indicates that the spaces should be <mark style="color:purple;">right-aligned</mark>, while the "12" indicates the width of the field, which is 12 characters. Finally, the empty string <mark style="color:purple;">""</mark> is used to <mark style="color:purple;">fill the field with spaces</mark>.
