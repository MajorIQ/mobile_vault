

Basic Graphical User Interface 

```java
import javax.swing.JOptionPane;

String name = JOPtionPane.showInputDialog("Enter your name"); // Creates a small GUI pop-up, to enter your name 

JOptionPane.showMessageDialog(null, "Hello " + name); // pop-up saying hello + name

int age = JOptionPane.showinputDialog("Enter your age"); // input GUI pop-up box - return a string 

/* 
convert GUI input into another data type 
int age = Integer.parseInt(JOptionPane.showinputDialog("Enter your age"));
*/

```


