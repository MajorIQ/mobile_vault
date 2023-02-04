
```ad-note
title: Exception Handling

An event occurs during the execution of a program that, disrupts the normal flow of instructions
```

```java
import java.util.Scanner;

public class Main {
	public static void main(String[] args) {

		Scanner scanner = new Scanner(System.in);

		System.out.println("Enter a whole number to divide: ");
		int x = scanner.nextInt();

		System.out.println("Enter a whole number to divide: ");
		int y = scanner.nextInt();

		int z = x / y;

		System.out.println("result: " + z);
		
	}
}
```

Try Block:

```java
try {

}
catch(ArithmeticException e) {
	System.out.println("You can't divide by zero! IDIOT!");
} 
```


Exception:

ArithmeticException - divide by zero
InputMismatchException // wrong data type

Exception e  - handles all exception

```java
try {

}
catch(ArithmeticException e) {
	System.out.println("You can't divide by zero! IDIOT!");
} 
finally {
	System.out.println("This will always print");
}
```


