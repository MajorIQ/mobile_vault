
```ad-note
title: Method Overriding

Declaring a method in sub class, which is already present in parent class.
- done so that a child class can give its own implementation
```

```java
public class Main {
	public static void main(String[] args) {
		Animals animal = new Animal();
		Dog dog = new Dog();
		
		dog.speak();
	}
}
```

```java
public class Animal {

	void speak() {
		System.out.println("The animal speaks");
	}
}
```

```java
public class Dog extends Animal {

	@Override // letting people know that this is an overriding method 
	void speak() {
		System.out.println("The dog goes bark");
	}

}
```


