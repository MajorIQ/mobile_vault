
| Modifier    | Class | Package | Subclass | World |
| ----------- | ----- | ------- | -------- | ----- |
| Public      | Y     | Y       | Y        | Y     |
| Protected   | Y     | Y       | Y        | N     |
| No modifier | Y     | Y       | N        | N     |
| Private     | N     | N       | N        | N     |

```java
package package1;
import package2.*;

// modules are visbale from other packages are class A is public 
public class A {
	public static void main(String[] args) {
		// TODO Auto-generate method stub

		C c = new C();
		System.out.println(c.defaultMessage)
	}
}
```

```java
package package1;
import package2.*;

public class B {

}
```

```java
package package2;
package package1.*;

public class C {
	public String publicMessage = "This is public";
	protected String protectedMessage = "This is protected";
		String defaultMessage = "This is the default";
	private String privateMessage = "This is private";
}
```

```java
package package2;
import package1.*;

public class Asub extends A {

	String defaultMessage = "This is the default";
}
```
