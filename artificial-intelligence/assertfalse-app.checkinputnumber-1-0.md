---
description: >-
  public void testCheckInputNumber() { assertTrue(App.checkInputNumber(1,100));
  assertFalse(App.checkInputNumber(1,0));
---

# 🍡 assertFalse(App.checkInputNumber(1,0))

The 'testCheckInputNumber' method tests the method by passing two sets of arguments and asserting whether the method returns 'true' or 'false'. The first assertion check if the method returns 'true' when passed the argemtns '1' and '100', while the second assertion if the mehod returns 'false' when passed the arguments'1' and '0'.

The `assertTrue` and `assertFalse` methods are JUnit assertion methods used to test whether a condition is true or false, respectively. The `assertTrue` method checks if a condition is true, while the `assertFalse` method checks if a condition is false[1](https://stackoverflow.com/questions/3241105/java-junit-asserttrue-vs-assertfalse)[2](https://coderolls.com/assertTrue-and-assertFalse-in-junit/)[5](https://www.lambdatest.com/blog/junit-assertions-example-for-selenium-testing/). If the condition is not satisfied, the assertion fails and an error message is displayed[1](https://stackoverflow.com/questions/3241105/java-junit-asserttrue-vs-assertfalse).In the provided JUnit test case, the `assertTrue` method is used to assert that the `checkInputNumber` method returns `true` when passed the arguments `1` and `100`. On the other hand, the `assertFalse` method is used to assert that the `checkInputNumber` method returns `false` when passed the arguments `1` and `0` [1](https://stackoverflow.com/questions/3241105/java-junit-asserttrue-vs-assertfalse)[2](https://coderolls.com/assertTrue-and-assertFalse-in-junit/).
