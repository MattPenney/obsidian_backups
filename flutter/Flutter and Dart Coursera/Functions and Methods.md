
Functions are reusable blocks of code that perform a specific task

Functions are declared with their return type

If the function does not return any data, the `void` keyword is used.

```dart
void printSomething() {
	print('Something');
}

int addNumbers(int num1, int num2) {
	return num1 + num2;
}

void main() {
	printSomething(); // Prints something
	int result = addNumbers(1, 2);
	print(result); // Prints 3
}
```


## Parameters 

Parameters are the pieces of data accepted when calling a function

Default values can be provided and arguments can be added

Parameter types include:
- Required
- Optional
- Named
- Default

### Required Parameters

Required and positional

```dart
int multiply(int a, int b) {
	return a * b;
}

void main() {
	print(multiply(3,4));
}
```

### Optional Parameters 

Can be positional or named

```dart
String fullName(String firstName, [String? middleName, String? lastName]) {
	return '$firstName ${middleName ?? ''} ${lastName ?? ''}';
}

void main() {
	print(fullName('John', 'Doe'));
	print(fullName('John', 'Paul', 'Doe'));
}
```

### Named Parameters

Specified using curly braces

Required or given default values

```dart
void greet({String name, String greeting = 'Hello'}) {
	print('$greeting, $name!');
}

void main() {
	greet(name: 'Alice');
	greet(name: 'Bob', greeting: 'Hi');
}
```

### Default Parameters

May be used with both positional and named parameters

## Arrow Functions

```dart
int square(int x) => x * x;

void main() {
	print(square(4)); // Output 16
}
```

## Methods

Methods are functions associated with an object

Defined within a class

Operate on instances of that class

Perform actions on data contained within objects

```dart
List<String> fruits = ['Apple', 'Banana', 'Cherry'];

fruits.add('Date');
print(fruits); 

fruits.remove('Banana');
print(fruits);

bool hasApple = fruits.contains('Apple');
print(hasApple);
```

## Closures

Allows functions to capture and store references to variables and their surrounding scope(lexical scope) even after the scope in which the variables were declared has finished executing



