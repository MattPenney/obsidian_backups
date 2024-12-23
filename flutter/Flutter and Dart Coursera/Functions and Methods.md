
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

