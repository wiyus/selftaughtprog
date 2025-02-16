**Inheritance** is an [[OOP]] concept in which a **[subclass](Subclass.md)** is created *inheriting* its methods from a **[superclass](Superclass)**. This means that an object of the *subclass* can call methods from the *superclass.*

# **Example**

```java
class Superclass {
	public void hello() {
		System.out.println("Hello, world!");
	}
}

class Subclass extends Superclass {
	/*Inherits the hello() method*/

	public void bye() {
		System.out.println("Goodbye, cruel world.");
	}
}

class Main {
	public static void main(String[] args) {
		Subclass sub = new Subclass();
		sub.hello(); /*Can call hello()*/
		sub.bye();
	}
}
```

An object from **Subclass** can call both the *hello()* method from **Superclass** and its own method *bye()*.