
```ad-note
title: While loop

Executes a block of code as long as a it's condition remains true
```

```java
Scanner input = new Scanner(System.in);
String name = "";

while(name.isBlank()) {
	System.out.println("Enter your name:  ")
	name = input.nextLine();
}
```

Do Loop (anyways executes once)

```java
Scanner input = new Scanner(System.in);
String name = "";

 do{
	System.out.println("Enter your name:  ")
	name = input.nextLine();
} while(name.isBlank());
```
