```ad-note
title: printf()

An optional method to control, format, and display text to the consol window
- two arguments = format string + (object/variable/value)
- % [flags] [precision] [width] [conversion-character]
```

```java
System.out.printf("%d This is a format string", 123) // 123 This is a format string
```

```java
boolean myBoolean = true;
char myChar = '@';
String myString = "Bro";
int myInt = 50;
double myDouble = 1000;

// boolean
System.out.printf("%b", myBoolean);

// Characters
System.out.printf("%c", myChar);

// Strings
System.out.printf("%s", myString);

// Integer
System.out.printf("%d", myInteger);

// Double / float
System.out.printf("%f", myDouble);



```

Width

minimum number of characters to be written as output 
```java
System.out.printf("Hello %10s",myString);
```

Precision

sets number of digits of precision when outputting floating-point values 

```java
System.out.printf("You have this much money %.1f",myDouble);
```

Flags

adds an effect to output based on the flag added to format specifier 
-: left-justify
+: output a plus ( + ) or minus ( - ) sign for a numeric value 
0 : numeric values are zero-padded 
, : comma grouping separator if numbers > 1000

```java
System.out.printf("You have this much money %,f",myDouble);
```
