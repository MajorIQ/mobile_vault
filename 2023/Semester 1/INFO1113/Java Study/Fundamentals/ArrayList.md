```ad-note
title: ArrayList

- A resizable array
- Elements can be added and removed after compilation phase
- store reference data type 
```


How to create a ArrayList 

```java
import java.util.ArrayList;

ArrayList<Reference data type/Wrapper class> ArrayList name = new ArrayList<data type>();
```

Example: 
```java
ArryaList<String> food = new ArrayList<String>();
```

How to add/ appends to an ArrayList

```java
ArryaList<String> food = new ArrayList<String>();

food.add("pizza")
food.add("hamburger")
food.add("hotdog")
```

How to iterate a display elements in a ArrayList

```java
ArryaList<String> food = new ArrayList<String>();

food.add("pizza")
food.add("hamburger")
food.add("hotdog")

for(int i = 0; i < food.size(); i++) {
	System.out.println(food.get(i))
}
```

Useful ArrayList Methods:

- Set Method
- Remove Method
- Clear Method

```java
// food.set(index, element); like the replace function
food.set(0, "sushi");

food.remove(2); // remove element 2

food.clear(); // removes all elements

```
