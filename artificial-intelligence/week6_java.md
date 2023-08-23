---
description: interface
---

# 🍡 Week6\_Java

To define an interface in Java, you use the `interface` keyword instead of `class`. An interface contains method signatures but no method bodies.

Interfaces define functionality that classes can implement. To implement an interface, a class uses the `implements` keyword:

```java
public class Dog implements Animal {

  @Override
  public void makeSound() {
    System.out.println("Bark!");
  }

  @Override
  public void eat() {
    System.out.println("The dog is eating"); 
  }

}
```

Implementing classes must override all methods declared in the interface and provide implementations for them. Interfaces allow for abstraction in Java since they define behaviors that classes can implement in different ways.

Some key properties of Java interfaces:

* Interface methods are implicitly public and abstract (no body)
* Variables defined in an interface are public, static and final by default
* A class can implement multiple interfaces using comma separation
* An interface can extend other interfaces

So in summary, interfaces define a contract that implementing classes must follow. This allows for abstraction and polymorphism.
