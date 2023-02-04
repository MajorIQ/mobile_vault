```ad-note 
title: Constructors

Speical method that is called when an object is instantiated (created)
```

```java
public class Main {
	public static void main(String[] args) {
		// create instance of the class by calling the class
		Humann human = new Human("Rick", 65, 70);
	}
}
```

create the constructor:

```java
public class Human {

	String name;
	int age;
	double weight;
	
	Human(String name, int age, double weight) {
		this.name = name;
		this.age = age;
		this.weight = weight;
	}
	void eat() {
		System.out.println(this.name + " is eating");
	}

	void drinking() {
		System.out.println(this.name + " is drinking");
		
	}
}
```

