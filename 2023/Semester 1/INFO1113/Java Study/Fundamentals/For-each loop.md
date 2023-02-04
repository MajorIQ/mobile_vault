
```ad-note
title: for-each

- Traversing technique to iterate through the elements in an array/collection
- less steps, more readable
- less flexible
```

Array
```java
String[] animals = {"cat", "dog", "bird"};

for(String i : animals) {
	System.out.println(i);
}
```

Collection: ArrayList
```java
import java.util.ArrayList;


ArrayList<String> animals = new ArrayList<String>();
animals.add("cat");
animals.add("dog");
animals.add("bird");

for(String i : animals) {
	System.out.println(i);
}

```
