# 🍡 Java concept of assignment 1

<mark style="color:red;">**JUnit**</mark> is a popular Java unit testing framework that is used to write and run repeatable automated tests. It is an open-source testing framework that allows Java programmers to create test cases and test their own code.

Some key features of JUnit include fixtures, test runners, and JUnit classes. Fixtures are methods that are run before and after each test code to set up and clean up the test environment. Test runners are used to execute test cases and report the results. JUnit classes are important classes used in writing and testing JUnits, such as the Assert class and the TestCase class.

**Example of fixtures:**

```java
import junit.framework.*;

public class JavaTest extends TestCase {
    protected int value1, value2;
    
    // assigning the values
    protected void setUp(){
        value1 = 3;
        value2 = 3;
    }
    
    // test method to add two values
    public void testAdd(){
        double result = value1 + value2;
        assertTrue(result == 6);
    }
}
```

**Examples of Test Suites:**

```java
import org.junit.runner.RunWith;
import org.junit.runners.Suite;

//JUnit Suite Test
@RunWith(Suite.class)

@Suite.SuiteClasses({
    TestJunit1.class ,TestJunit2.class
})

public class JunitTestSuite{
}
```
