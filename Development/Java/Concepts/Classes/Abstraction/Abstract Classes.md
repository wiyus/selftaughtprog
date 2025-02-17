An [[Abstract]] [[Class]] can use [[Abstract Methods]] alongside regular [[method]]s.

You **cannot create** an object from abstract class, it must be **[extended](Inheritance.md)** from a class.

# **Example**

```java
abstract class Animal {
	public abstract void makeSound(); /*Abstract Method*/
	public void sleep() { /*Regular Method*/
		System.out.println("Zzz");
	} 
}

class Chicken extends Animal {
	public void makeSound() { /*view [[Abstract Methods]]*/
		System.out.println("Bawk!");
	}

	/*sleep() is provided*/
}

class Main {
	public static void main(String[] args) {
		Chicken chicken = new Chicken();
		chicken.sleep(); /*-> Zzz*/
		chicken.makeSound(); /*-> Bawk!*/
	}
}
```

