---
description: 20/08/2023 study
---

# 🍡 HashSet

HsahSet is a class that implements the set interface and uses a hash table to store elements. It is a collection that contains unique elements and does not allow duplicates.

And hash set allows null values.



```java
import java.util.HashSet;
public class HashSetExample {
    public static void main(String[] args) {
        HashSet<String> set = new HashSet<>();
        
        set.add("Apple");
        set.add("Banana");
        set.add("Orange");
        
        System.out.println(set); // output:[Apple, Banana, Orange]
        set.remove("Banana");
        System.out.println(set); // output:[Apple, Orange]
        System.out.println(set.contains("Apple")); // output: true
        System.out.println(set.size()); output:2
        
    }
}
```

^= operator

It is used to perform a bitwise XOR operation on the two operands and assign the result to the left operand.

If we have the expression 'a ^=b', it is equivalent to 'a=a^b', where 'a' and 'b' are variables.

The XOR operation returns a 1 in each bit position where the corresponding bits of either but not both operands are 1s. Therefore, using the '^=' operator can be useful for manipulating and toggling specific bits in a binary representation.



```java
int a = 5; // binary: 0101
int b = 3; // binary: 0011

a ^= b; // a = a ^ b

System.out.println(a); // Output: 6 (binary: 0110)
```

In computer science, time complexity and space complexity are used to analyze the efficiency and performance of algorithms. They help us understand how the runtime and memory usage of an algorithm changes as the input size grows.

1. Time complexity (O(n)): Time complexity refers to how much time an algorithm takes to solve a problem. It is typically expressed as a function of the input size of the problem. The most common notation used to describe time complexity is Big O notation. The "O" in Big O stands for "order of" and represents the upper bound of the algorithm's time complexity. The "n" in O(n) represents the input size.

O(1)- Constant Time complexity: An algorithm with constant time complexity takes the same amount of time to run, regardless of the input size. It means that the runtime of the algorithm does not depend on the size of the input. For example, accessing an element in an array by index or performing a simple arithmetic operation takes constant time.

O(n)- Linear Time Complexity: An algorithm with linear time complexity has a runtime that grows linearly with the input size. It means that the runtime of the algorithm is directly proportional to the size of the input. For example, iterating through an array or performing a linear search has a linear time complexity.

2. Space Complexity (O(1)): Space complexity measures how much memory an algorithm uses  to solve a problem. It is also expressed using Big O notation. The "1" in O(1) represents constant space complexity, which means that the amount of memory used by the algorithm does not depends on the input size.

Space Complexity (O(1)): Space complexity measures how much memory an algorithm uses to solve a problem. It is also expressed using Big O notation. The "1" in O(1) represents constant space complexity, which means that the amount of memory used by the algorithm does not depend on the input size.

O(1) - Constant Space Complexity: An algorithm with constant space complexity uses a fixed amount of memory, regardless of the input size. It means that the memory usage of the algorithm remains constant. For example, storing a few variables or a fixed-size array has constant space complexity.

To summarize, **O(n)** represents **linear time complexity**, where the **runtime** of an algorithm grows linearly with the input size. **O(1)** represents **constant space complexity**, where **the memory usage** of an algorithm remains constant regardless of the input size.
