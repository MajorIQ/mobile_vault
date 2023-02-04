
```ad-note
title: Objects 

An instance of a class that may contain attributes and methods 

Exampels: Phone, desk, computer, coffee cup 
```

Attributes = The different characteristics an object have 
Methods = The different actions the object have

Creating Class
```java
public class Car {

	// car attributes
	String make = "Chevrolet";
	String model = "Corvette";
	int year = 2020;
	String color = "blue";
	double price = 50000.00;

	// drive method
	void drive() {
		System.out.println("You drive the car");
		}

	// brake method
	void brake() {
		System.out.println("You step on the brakes");
	}
}
```

How to construct an instances of another class
constructing an object 

```java
public class Main {
	public static void main(String[] args) {

	// creating car object - instance of the Car class 
	Car myCar = new Car();

	// printing object attributes
	System.out.println(myCar.make);
	System.out.println(myCar.model);

	// calling class method 
	myCar.drive();
	myCar.brake();
	}
}
```

