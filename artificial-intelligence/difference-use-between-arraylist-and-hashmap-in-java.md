# 🍡 difference use between ArrayList and HashMap in Java

An example:&#x20;

When you want to iterate every element in ArrayList:



```java
ArrayList<Character> Mylist = new ArrayList<Character>();
        for (char element : magazine.toCharArray()) {
            Mylist.add(element);
        }
```

When you want to iterate every element in HashMap:



```java
HashMap<Character, Integer> charFreq = new HashMap<>();
    for (char c : magazine.toCharArray()) {
        charFreq.put(c, charFreq.getOrDefault(c, 0) + 1);
    }
```

**Example 1:**

<pre><code><strong>Input: ransomNote = "a", magazine = "b"
</strong><strong>Output: false
</strong></code></pre>

**Example 2:**

<pre><code><strong>Input: ransomNote = "aa", magazine = "ab"
</strong><strong>Output: false
</strong></code></pre>

**Example 3:**

<pre><code><strong>Input: ransomNote = "aa", magazine = "aab"
</strong><strong>Output: true
</strong></code></pre>

Option 1: Use ArrayList:



```java
class Solution {
    public boolean canConstruct(String ransomNote, String magazine) {
        if (ransomNote.length() > magazine.length()) {
            return false;
        }
        ArrayList<Character> Mylist = new ArrayList<Character>();
        for (char element : magazine.toCharArray()) {
            Mylist.add(element);
        }
        for (char i : ransomNote.toCharArray()) {
            if (Mylist.contains(i)) {
                Mylist.remove((Character) i);    
            } else {
                return false;
            }
        }
        return true;
    }
} 
```

Option2: Use HashMap:



```java
public boolean canConstruct(String ransomNote, String magazine) {
    if (ransomNote.length() > magazine.length()) {
        return false;
    }
    HashMap<Character, Integer> charFreq = new HashMap<>();
    for (char c : magazine.toCharArray()) {
        charFreq.put(c, charFreq.getOrDefault(c, 0) + 1);
    }
    for (char c : ransomNote.toCharArray()) {
        if (charFreq.containsKey(c) && charFreq.get(c) > 0) {
            charFreq.put(c, charFreq.get(c) - 1);
        } else {
            return false;
        }
    }
    return true;
}
```
