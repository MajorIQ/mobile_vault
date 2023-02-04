
```ad-note
title: File

An abstract representation of file and directory pathnames
```

```java
import java.io.File;

public class Main {
	public static void main(String[] args) {
		File file new File("File name");

		if(file.exists()) {
			System.out.println("that file exists! :0!")
			System.out.println(file.getPath()); // display path of file
			System.out.println(file.getAbsolutePath()); // displays absolute path
			System.out.println(file,isFile()); // displays if file is a file
			file.delete(); // delete this file 
		}
		else {
			System.out.println("that file doesn't exist ! :0!")
			
		}
	}
}
```
