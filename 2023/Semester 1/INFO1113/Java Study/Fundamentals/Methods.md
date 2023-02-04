
```ad-note
title: Method

A block of code that is executed whenever it is called upon 

```

```java
public class Main { 
	public static void main(String[] args) { 
	int x = 3;
	int y = 4; 
	
	int z = add(x,y);
	System.out.println(z); 
	} 

static int add(int x, int y) { 
	int z = x + y; return z; 
	} 
}
```

static = It belongs to the class, rather than a specific instance
void  = Returns Nothing
