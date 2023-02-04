
```ad-note 
title: Encapsulation

- Attributes of a class will be hidden or private
- Can be accessed only through methods (getters & setters)
- You should make attributes private if you don't have a reason to make them public/protected
```

```java
public class Main {
	public static void main(String[] args) {
		Car car = new Car("Chevrolet", "Camaro", 2021);
	}
}
```

```java
System.out.println(car.make);
```

Can't access private variables from another class

```java
public class Car {
	private String make;
	private String model;
	private int year;

	Car(String make, String model, int year) {
		this.make = make;
		this.model = model;
		this.year = year;
	}
}
```

Fix - Getter Method 

```java
// Getter method
public String getMake() {
	return make;
}
public String getModel() {
	return model;
}
public int getYear() {
	return year;
}
```

Calls getter method instead of access the object attribute directly 

```java
System.out.println(car.getMake());
System.out.println(car.getModel());
System.out.println(car.getYear());

```

How to change private attributes of an object

Fix - Setter Method

```java
public void setMake(String make) {
	this.make = make;
}
public void setModel(String model) {
	this.model = model;
}
public void setYear(int year) {
	this.year = year;
}
```

Therefore we can use our setter methods to assign our object attributes
```java
public class Car {
	private String make;
	private String model;
	private int year;

	Car(String make, String model, int year) {
		this.setMake(make);
		this.setModel(model);
		this.setYear(year);
	}
}
```
