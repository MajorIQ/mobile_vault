

```java
public class Main {
	public static void main(String[] args) {

		// creating array
		int[] numbers = new int[3];
		char[] characters = new char[4];
		String strings = new String[5];

		// declaring an array of food objects
		Food[] refrigerator = new Food[3];

		Food food1 = new Food("pizza");
		Food food1 = new Food("hamburger");
		Food food1 = new Food("hotdog");
	
		// creating an array of objects
		Food[] refrigerator = {food1, food2, food3};

		// stores object inside an array
		refrigerator[0] = food1;
		refrigerator[1] = food2;
		refrigerator[2] = food3;

		System.out.println(refrigerator[0].name)
	}
}
```

```java
public class Food {
	String name;

	Food() {
	this.name = name;
	}

}
```
