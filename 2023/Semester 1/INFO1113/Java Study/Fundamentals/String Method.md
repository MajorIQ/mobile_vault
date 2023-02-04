```ad-note
title: String

Is a referance data type that can store one or more characters, reference data type have acess to useful methods
```


Equals Method - Returns Boolean 
```java
String name = "Bro";

boolean result = name.equals("Bro"); // Case sensitive 

boolean result = name.equalsIgnoreCase('bro'); // non-Case sensitve

System.out.println(result); 
```

Length Method - Returns Integer

```java
String name = "Bro";

int result = name.length(); 

System.out.println(result); 
```


charAt  Method - Returns single character

```java
String name = "Bro";

char result = name.charAt();

System.out.println(result); 
```

indexOf - Returns integer

```java
String name = "Bro";

char result = name.indexOf("B");

System.out.println(result); // B
```

isEmpty - Returns boolean

```java
String name = "Bro";

boolean result = name.isEmpty();

System.out.println(result); 
```

isBlank - Returns boolean

```java
String name = "  /t /n    ";

boolean result = name.isBlank();

System.out.println(result); // True
```


toUpperCase - Returns String

```java
String name = "Bro";

String result = name.toUpperCase();

System.out.println(result); // BRO
```

toLowerCase - Returns String

```java
String name = "Bro";

String result = name.toLowerCase();

System.out.println(result); // bro
```

trim - Returns String

```java
String name = "    Bro    ";

String result = name.trim();

System.out.println(result); // Bro   - removes empty space before and after string
```

replace - Returns String

```java
String name = "Bro";

String result = name.repalce('o', 'a');

System.out.println(result); // Bra
```