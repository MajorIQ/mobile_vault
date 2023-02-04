create new file and write
write

append to existing file
append 
```java
import java.io.FileWriter; 
import java.io.IOException;

public class Main {
	public static void main(Sring[] args) {
		try {
			FileWriter writer = new FileWriter("file path");
			writer.write("ROses are red \nViolets are blue\nBooty booty booty booty \nRockin' everywhere!")
			writer.close();
		}
		catch (IOException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		} 
		
	}
}
```
