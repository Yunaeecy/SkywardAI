# 🍡 HashSet

HsahSet is a class that implememts the set interface and uses a hash table to store elements. It is a collection that contains unique elements and does not allow duplicates.

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
