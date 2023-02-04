```ad-note
title: Array

used to store multiple values in a single variable 

```

```java
String[] cars = {"Camaro", "Corvette", "Tesla"};

cars[0] = "Mustang"; // replaces index 0 of cars array to mustang 

```

Another way to make an array
```java
String[] cars = new String[3];

cars[0] = "Camaro"
cars[1] = "Corvette"
cars[2] = "Tesla"
```

To iterate elements of an array 

```java
for(int i = 0, i < cars.length, i++) {
	System.out.println(cars[i]);
}
```
