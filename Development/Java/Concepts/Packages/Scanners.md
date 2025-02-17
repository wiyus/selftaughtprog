**Scanners** come from the java util package:

```java
import java.util.Scanner; 
```

To use them, you must create a new **Scanner** [[Class|class]] object within the class you want to use it in.

```java
Scanner <name> = new Scanner(System.in);
```

**Methods** of this object include:


| Method               | Description                              |
| -------------------- | ---------------------------------------- |
| ```nextLine()```<br> | Read a ```String``` value from the user  |
| ```nextBoolean()```  | Read a ```boolean``` value from the user |
| ```nextByte()```     | Read a ```byte``` value from the user    |
| ```nextDouble()```   | Read a ```double``` value from the user  |
| ```nextFloat()```    | Read a ```float``` value from the user   |
| ```nextInt()```      | Read an ```int``` value from the user    |
| ```nextLong()```     | Read a ```long``` value from the user    |
| ```nextShort()```    | Read a ```short``` value from the user   |
|                      |                                          |
# Example

```java
import java.util.Scanner;

class Main {
	public static void main(String[] args) {
		/*Instantiate Scanner object*/
		Scanner myScanner = new Scanner(System.in);

		System.out.println("Insert your name: ");
		String name = myScanner.nextLine();

		System.out.println("Your name is " + name);
	}
}
```

