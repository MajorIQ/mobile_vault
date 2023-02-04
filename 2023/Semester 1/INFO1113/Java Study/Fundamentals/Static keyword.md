
```ad-note
title: Static Keyword

Modifier. A single copy of a variable/method is created and shared.

- The class 'owns' the static member
```

```java
public class Main {
	public static void main(String[] args) {
		Friend friend1 = new Friend("Sponegbob");
		Friend friend2 = new Friend("Patrick");
		Friend friend3 = new Friend("Squidward");
		
		System.out.println(Friend.numberOfFriends);

		Friend.displayFriends();

		Math.round(a); // static method
	}
}
```



```java
public class friend {

	String name;
	static int numberOfFriends; 
	
	Friend(String name) {
		this.name = name;
		numberOfFriends++;
	}
	static void displayFriend() {
		System.out.println("You have " + numberOfFriends + " friends");
	}
}
```

