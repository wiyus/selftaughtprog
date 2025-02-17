**Encapsulation** is the [[OOP]] process of rendering "sensitive data" [[private]] and allowing it to be updated only using **getter** and **setter** methods. This allows developers to restrict the possible values of the private object, for instance.

# **Example**

```java
public class BankAccount {
	private double balance;

	public void setBalance(double balance) {
		if (balance >= 0) { /*prevents negative balances*/
			this.balance = balance;
		} else {
			System.out.println("Invalid");
		}
	}

	public double getBalance() {
		return this.balance;
	}
}
```

