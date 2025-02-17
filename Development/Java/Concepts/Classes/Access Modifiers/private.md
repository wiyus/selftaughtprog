Usable for everything **but** classes (see [[Inner Class|inner classes]], **private** means the element is only accessible within the class it's declared in.

```java
class First {
	private int number = 0;
	public int doubleNumber = this.number*2;
}

class Second {
	public int copy = number; /*won't work*/
}

class Main {
	public static void main(String[] args) {
		First first = new First();
		System.out.println(first.number); /*won't work*/
	}
}
```

