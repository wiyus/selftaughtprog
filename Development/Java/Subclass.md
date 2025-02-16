The child of a **[superclass](Superclass.md)**, the class *[inheriting](Inheritance)* from the other.

You can call upon the *superclass* with the **super** keyword.

# **Example**

```java
class Weight {
	int weight = 10;
	
	public void showWeight() {
		System.out.println("The weight is " + weight + "kgs.");
	}
	
	public void showWeight(int w) {
		System.out.println("The weight is " + w + "kgs.");
	}
}

class DoubleWeight extends Weight {
	public void showWeight() {
		super.showWeight(super.weight*2);
	}
}

class Main {
	public static void main(String[] args) {
		Weight w = new Weight();
		DoubleWeight w2 = new DoubleWeight();
		w.showWeight();
		w2.showWeight();
	}
}
```