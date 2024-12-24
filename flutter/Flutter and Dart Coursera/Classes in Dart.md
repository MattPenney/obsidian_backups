#dart #coursera 

A class is a blueprint

An instance of this class is the object

A class defines properties and behaviours

Each object has a unique state

## Properties

Represent data

```dart
class Person {

	//Public properties
	String name;
	int age;
	
	//Private property
	String _ssn;
	
	//Constructor
	Person(this.name, this.age, this._ssn);
	
	//Method
	void displayInfo() {
		print('Name: $name, Age: $age, SSN:$_ssn');
	}
}
```

### public

Allows access by external classes
### private

Controls access

Can only be accessed from within the class

An underscore declares a private property


## Methods

Represent behaviour

```dart
class Person {
	String name;
	int age;

	Person(this.name, this.age);

	void describe() {
		print('I am $name and I am $age years old.');
	}

	int yearsUntilRetirement() {
		return 65 - age;
	}
}

void main() {
	Person p = Person('Alice', 30);
	p.describe(); // Output: 'I am Alice and I am 30 years old.'
	print(p.yearsUntilRetirement()); // Output: 35
}
```

### Getters and Setters

#### Getters

Perform calculations or formatting

Uses `get` keyword

```dart
class Circle {
	double radius;
	
	Circle(this.radius);

	double get area => 3.14 * radius * radius;
}

void main() {
	Circle c = Circle(5);
	print(c.area);
}

class Rectangle {
	double _width = 0;
	double _height = 0;

	void set width(double value) {
		if (value > 0) {
			_width = value;
		}
	}

	void set height(double value) {
		if (value > 0) {
			_height = value;
		}
	}

	double get area => _width * _height;
}

void main() {
	Rectangle r = Rectangle();
	r.width = 10;
	r.height = 20;
	print(r.area); //Output: 200

}
```

#### Setters 

Validate input or trigger actions

### Static Methods

Do not belong to object instances

Used for utility functions

Don't require access to object-specific data

Examples:
- Utility conversions
- Mathematical calculations

```dart
class Math {
	static double pi = 3.14;

	static int square(int x) {
		return x * x;
	}
}

void main() {
	print(Math.pi); // Output: 3.14
	print(Math.square(4)); //Output: 16	
}
```

### Anonymous Functions

Nameless and ideal for short, one time operations

Offers flexibility--can be passed to other functions, etc

Promotes clean code for complex programs

```dart

void main() {
	var list = ['apples', 'bananas', 'oranges'];
	list.forEach((item) {
		print(item);
	});
}
```

## Encapsulation

Protects data from unauthorized access

The keys are getters and setters

```dart

class BankAccount {
	String _accountNumber;
	double _balance;

	BankAccount(this._accountNumber, this._balance);

	double get balance => _balance;

	void deposit(double amount) {
		if (amount > 0) {
			_balance += amount;
		}
	}

	void withdraw(double amount) {
		if (amount <= balance) {
			_balance -= amount;
		} else {
			print('Insufficient funds');
		}
	}
}

void main() {
	BankAccount account = BankAccount('123456789', 1000.0);
	print('Balance: \$${account.balance}'); // Output: Balance: 1000.0
}
```

## Iherit


