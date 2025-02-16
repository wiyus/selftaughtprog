Usable for everything **but** classes. **protected** means the element may be accessed within the same [package](Packages) or by [subclasses](Inheritance).

# Example

```java
//src/packageOne/FileOne.java

class FileOne {
	protected static String password() {
		return "1234";
	} 
}
```

```java
//src/packageTwo/FileTwo.java

import packageOne.FileOne;

class FileTwo extends FileOne {
	public String publicPassword() {
		return password(); /*inherited from FileOne*/
	}
}

class FileThree {
	public String publicPassword() {
		return password(); /*won't work*/
	}
}
```
