A **class** is an object with **attributes** and **methods**. Its purpose is to conceive **objects.**

# Example

```java
public class MyClass {
	public String attribute = "This is an attribute";

	public void method() {
		System.out.println("This is a method");
	}
}

public class Main {
	public static void main(String[] args) {
		MyClass myClass = new MyClass();
		System.out.println(myClass.attribute);
		myClass.method();		
	}
}
```
