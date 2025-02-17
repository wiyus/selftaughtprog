An **interface** is an **[[Abstract Classes|abstract class]]** of which all methods are [[Abstract Methods|abstract methods]]. It is, however, not **[[Inheritance|inherited]]**, but **implemented**, and unlike inheritance, you can **implement multiple interfaces.**

# Example

```java
interface Animal {
	public void animalSound();
	public void sleep();
}

interface Breedable {
	public void breed();
}

class Cat implements Animal, Breedable { /*two interfaces*/
	@Override
	public void animalSound() { /*from Animal*/
		/*method definition*/
	}

	@Override
	public void sleep() { /*from Animal*/
		/*method definition*/
	}

	@Override
	public void breed() { /*from Breedable*/
		/*method definition*/
	}
	/*Above methods are enforced*/

	public void leaveHouse() {
		/*method definition*/
	}
	/*Above method is exclusive to Cat (not part of any interface)*/
}
```