An **inner class** is a class within another class (a **nested** class). Nesting classes that belong together helps with **code clarity.**

A **nested class** may be either [[private]] or [[protected]].

# Example

```java
class One {
	int x = 5;
	
	class Two {
		int y = 10;
	}
	
	private class Three {
		int z = 15;
	}
}

public class Main {
	public static void main(String[] args) {
		One one = new One();
		One.Two two = One.new Two();
		One.Three three = One.new Three(); /*won't work, Three is private*/
		System.out.println(one.x + two.y);
		System.out.println(one.x + three.z); /*won't work*/
	}
}
```
