
```ad-note
title: Polymorphism

- Greek work for poly-"many", morph-"form"
- The ability of an object to identify as more than one tpye
```

```java
public class Main {
	public static void main(String[] args) {

		Car car = new Car();
		Bicycle bicycle = new Bicycle();
		Boat boat = new Boat();

		Vehicle[] racers = {car, bicycle, boat}

		// Could do
		car.go();
		bicycle,go();
		boat.go();

		// Better solution
		for(Vehicle x : racers) {
			x.go()
		} 
	}
}
```


```java
public Vehicle {

}
```

```java
@Override
public Car extends Vehicle {
	public void go() {
		System.out.println("The car begins moving")
	}

}
```

```java
@Override
public Bicycle extends Vehicle {
	public void go() {
		System.out.println("The bicycle begins moving")
	}

}
```

```java
@Override
public Boat extends Vehicle {
	public void go() {
		System.out.println("The boat begins moving")
	}

}
```




