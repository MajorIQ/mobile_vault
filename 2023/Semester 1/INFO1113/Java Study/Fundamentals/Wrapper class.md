
```ad-note
title: Wrapper Class 

Provides a way to use primitve data types as reference data types, reference data types contain useful methods that can be used with collections (ex.ArrayList)
```

| Advantages             | Disadvantages |
| ---------------------- | ------------- |
| Contain useful methods | Slower to access              |
| Used in collections. i.e. ArrayList                       |               |

Wrapper class to make a reference data type 

| Primitive | Wrapper |
| --------- | ------- |
| boolean   | Boolean |
| char      | Character        |
| int       | Integer |
| double    | Double  |

```ad-note
title: Autoboxing

The automatic conversion that the Java comiler makes between the primitive data types and their corresponding object wrapper class
```

```java
Boolean a = true;
Character b = '@';
Integer c = 123;
Double d = 3.14;
String e = "Daniel" // Reference data type 
```


```ad-note
title: Unboxing

The reverse of autoboxing. Automatic conversion of wrapper class to primitive 
```