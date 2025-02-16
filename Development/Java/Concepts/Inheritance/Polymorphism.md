**Polymorphism** is an [[OOP]] concept which extends upon [inheritance](Inheritance). It involves **overriding** an instance of a [superclass'](Superclass) method within a [subclass](Subclass).

# **Example** 

```java
class Animal {
	public void makeSound() {
		System.out.println("Generic sound.");
	}
}

class Cat extends Animal {
	@Override /*Optional*/
	public void makeSound() { /*Overrides Animal's makeSound()*/
		System.out.println("Meow!");
	}
}
```

You can **expand** on the **superclass**' method rather than replace it by calling said method using **super.*<method_name>*** before any additions.


```java
class Animal {
	public void makeSound() {
		System.out.println("Generic sound.");
	}
}

class Cat extends Animal {
	@Override /*Optional*/
	public void makeSound() { 
		super.makeSound(); /*Animal's makeSound() method*/
		System.out.println("Meow!");
	}
}
```