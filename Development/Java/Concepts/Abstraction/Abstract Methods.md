Part of [[Abstract Classes]], using an **Abstract Method** forces all [subclasses](Inheritance) of the **Abstract Class** to [implement](Polymorphism) it.

# **Example:**

```java
abstract class Animal {
	abstract void makeSound();
}

class Cat extends Animal {
	@Override /*optional*/
	void makeSound() {
		System.out.println("Meow!)
	}
}```

If the **Cat** class didn't implement **makeSound()**, there would be an error.
