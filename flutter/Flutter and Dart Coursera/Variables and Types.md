#dart #coursera 

## Variable Declaration

Variables act as placeholders for storing data

Data types specify which kind of data a variable can hold

Variables must be declared and given a value

```dart
	var variable = 3;
```
Can be declared with the keywords `var` `const` or `final`

### var

var declares a variable without explicitly specifying a data type

The data type will be inferred 

The variable can then be reassigned to another value of the same type

### const

Compile time constant

Cannot be changed

### final

Set at runtime

Once it is set, it cannot be changed

## Data Types

Statically typed so every variable must have a type

Types include 
- Numbers
	- int
	- double
- Strings
- Booleans
- Lists
- Maps

### Numbers

Includes ints and doubles

### Strings

May use single or double quotes 

```dart
"String"
'Also a string'
```

Uses string interpolation -- a variable or expression may be included inside of a string

```dart
var variable = 'world'
'Hello $variable!'
```


### Booleans

 Represents true or false

Used in control flow statements

### Lists

Ordered collection of items

0 indexed

```dart
List<String> fruits = ['Apple', 'Banana', 'Cherry'];
print(fruits[0]);

fruits.add('Orange');
```

### Maps

Collection of key value pairs

Keys must be unique

```dart
Map<String, int> scores = {
	'Alice': 90,
	'Bob': 85,
	'Charlie': 95,
};

print(scores['Alice']);

scores['Dave'] = 80;
```

### null

Not initialized

```dart
String? nullString = null;
```

### Type Inference and Annotation

#### Inference

```dart
var city = 'New York';
```

#### Annotation

```dart
String country = 'USA';
```

