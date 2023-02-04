
```ad-note
title: Overloaded Constructors

- Multiple constructors within a class with the same name, but have different parameters
- name + parameters = signature
```

```java
public class Main {
	public static void main(String[] args) {
		Pizza pizza = new Pizza("thicc crust", "tomato", "mozzerella", "pepperoni" );
	System.out.print("Here are the ingredients of your pizza: ");
	System.out.print(pizza.bread);
	System.out.print(pizza.sauce);
	System.out.print(pizza.chesse);
	System.out.print(pizza.topping);

	}

}
```

```java
public class Pizza {

	String bread;
	String sauce;
	String chesse;
	String topping;

	// overloaded constructor, different parameters
	Pizza(String bread) {
		this.bread = bread;

	// overloaded constructor, different parameters
	Pizza(String bread, String sauce) {
		this.bread = bread;
		this.bread = sauce;

	// overloaded constructor, different parameters
	Pizza(String bread, String sauce, String chesse) {
		this.bread = bread;
		this.bread = sauce;
		this.bread = chesse;
	
	Pizza(String bread, String sauce, String chesse, String topping) {
		this.bread = bread;
		this.bread = sauce;
		this.bread = chesse;
		this.bread = topping;
		
	}
}
```
