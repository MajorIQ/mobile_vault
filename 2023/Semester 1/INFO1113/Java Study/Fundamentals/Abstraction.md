
```ad-note
title: Abstract 

- Abstract classes cannot be instantiated, but they can have subclass
- Abstract methods are declared without an implementation
```

```java
public class Main {
	public static void main(String[] args) {

		Vehicle vechile = new Vehicle();
		Car car = new Car();

		car.go();
		
	}
}
```

```java
// abstact keyword prevents creation of insistance
public abstract class Vehicle {

	abstract void go();
	}
}
```

```java
public class Car extends Vehicle {

	@Override
	void go() {
		System.out.println("The driver is driving the car")

}
```
