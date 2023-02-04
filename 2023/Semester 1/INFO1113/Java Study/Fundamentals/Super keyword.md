
```ad-note
title: Super Keyword

Refers to the superclass (parent) of an object
- very similar to the "this" keyword
```

```java
public class Main {
	public static void main(String[] args) {

	Hero hero1 = new Hero("Batman", 42,"$$$");
	Hero hero2 = new Hero("Superman", 43,"everything");
	
	System.out.println(hero1.name);
	System.out.println(hero1.age);
	System.out.println(hero1.power);

	System.out.println(hero2.toString());
	}
}
```

```java
public class Person {
	
	String name;
	int age;

	Person(String name, int age) {
		this.name = name;
		this.age = age;
	}
	public String toString() {
		return this.name + "\n" + this.age + "\n"
	}
}
```

```java
public class Hero extends Person {

	String power;

	Hero(String name, int age, String power) {

		super(name, age);
		this.power = power;
	}
	public String toString() {
		return super.toString() + this.power;
	}
}
```


