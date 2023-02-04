
```ad-note
title: 2D Array

an array of arrays; has rows and columns
```

```java
String[][] cars = {
	{"Camaro", "Corvette", "Silverado"},
	{"Mustang", "Ranger", "F-150"},
	{"Ferrari", "Lambo", "Tesla"}
				  }; 
	

```

Another way to create a 2D Array

```java
String[][] cars = new String[3][3];

cars[0][0] = "Camaro";
cars[0][1] = "Corvette";
cars[0][2] = "Silverado";
cars[1][0] = "Mustang";

```

To iterate and print elements of an 2D array

```java
for(int i = 0; i < cars.length; i++) {
	System.out.println();
	for(int j = 0; j < cars[i].length, j++) {
		System.out.println(cars[i][j] + " ")
	}
}
```
