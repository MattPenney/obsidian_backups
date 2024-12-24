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
	p.describe

}
```