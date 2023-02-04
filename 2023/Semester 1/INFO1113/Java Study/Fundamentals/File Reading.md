
```ad-note
title: File Reader

Read the contents of a file as a stream of characters. One by one read() returns an int value which contains the byte value when read() returns -1, there is no more data to read
```

```java
import java.io.FileReader; 

public class Main {
	public static void main(String[] args) {

		try {
			FileReader reader = new FileReader("File path");
			int data = reader.read();
			while(data != -1) {
				System.out.print((char)data);
				int data = reader.read();
			}
			reader.close()
		}
		catch (FileNotFoundException e) {
			e.printStackTrace();
		}
		catch (IOException e) {
			e.printStackTrace();
		}
	}
}
```
