# Coding Fundamentals

## Variables 
  - Used to store different types of information.
```
String name = "dolphin";
int age = 20;
double pi = 3.14;
bool isBeginner = true;
```

## Basic Math Operators

```
1 + 1 -> 2 add
4 - 3 -> 1 sub
2 * 3 -> 6 multiply
8 / 4 -> 2 divide
9 % 4 -> 1 reminder
++ -> increment by 1
-- -> decrement by 1
```

## Comparison Operators
	
```
5 == 5 -> true EQUAL TO
2 != 1 -> true NOT EQUAL TO
3 > 2 -> true GREATER THAN
3 < 2 -> false LESS THAN 
4 >= 2 -> true GREATER THAN OR EQUAL TO
4 <= 2 -> false LESS THAN OR EQUAL TO
```  

## Logical Operators

- AND operator(&&), 
  - returns true if both sides are true
  - isBeginner && (age < 68) -> returns false
- OR operator(||)
  - returns true if any one side is true
  - isBeginner || (age < 68) -> return true
- NOT operator(!), 
  - returns the opposite value
  - !isBeginner -> returns false
		
## if-else Statements

- Syntax

#### Only if statement
```
if (condition) 
{
	<do something babe>
}
```

#### if with else statement
```
if (condition) 
{			
	<do something>
} 
else 
{
  <do another thing>
}
```

#### if with else if statement
```
if (condition) 
{
  <do something babe>
} 
else if (condition) 
{
  <risk something babe>
}
```

#### if with else if and else statement

```
if (condition) 
{
  <do something>
} 
else if (condition) 
{
  <say something babe>
} 
else
{
  <risk something babe>
}
```
- Example
```
String grade = "A";

if (grade == "A") 
{
  print("Excellent");
} 
else if (grade == "B") 
{
  print("Good");
}
else if (grade == "C") 
{
  print("Average");
}
else if (grade == "F") 
{
  print("Fail");
}
else 
{
  print("Invalid grade");
}
```

## Switch Statement

- Syntax
```
switch (expression) {
	case value:
		break;
	default:
}
```

- Example
```
String song = "Fuck it i love you";

switch (song) {
	case "Fuck it i love you":
	  print("NFR");
	  break;
	case "Dark paradise":
	  print("Born to die");
	  break;
	case "Sad girl":
	  print("Ultraviolence");
	  break;
	case "Religion":
	  print("Honeymoon");
	  break;
	case "Lust for life":
	  print("Lust for life");
	  break;
	default:
	  print("Invalid song");
}
```

## Loops

###  for loop

- If you know how many times to iterate or loop you can use for loops

- imagine you have a playlist with 10 songs and you want to play each one after the another,
for each song in playlist, play that perticular song from playlist.

- continue -> skips the current iteration
- break -> break out of the loop

- Syntax
```
for(initialization; condition; increment_the_iterator){
	//RISK SOMETHING BABE
}
```
- Example 1
```
for (var i = 0; i < 10; i++) {
	print(i);
}
```

- Example 2 (with if statement)
```
for (var i = 0; i < 10; i++) {
	if (i != 4) continue;
	print(i);
}
```

### While loop

- If you dont know how many times to iterate you can use while loops

- Syntax

```
while (condition) {}
```

- Example

```
int countDown = 5;
while (countDown > 0) {
	print(countDown);
	countDown--;
}
```

## Functions

- Functions are self contained set of statement that perform a desired task
- Calling a function - `function_name(parameters_if_any)`

#### Functions without parameters
```
void greet() {
	print("Hello, welcome!");
}
```

#### Functions with parameters
```
void greetPerson(String name) {
	print("Hello, ${name} Welcome!");
}
```
- `name` -> is the parameter for this function.
- when you call this function e.i, `greetPerson("dolphin")`, you need supply a string value to the function.
	
#### Functions with void return type
```
void printName(String name) {
	print(name);
}
```

#### functions with return type
- Integer return type

```
int Add(int a, int b) {
	int result = a + b;
	return result;
}
```

- String return type

```
String getName(int id) {
  if (id == 1) {
	  return "Kyle";
  }
  return "Invalid ID";
}
```

- Boolean return type
```
bool isValidUser(int id, String name) {
	if (id != 1 && name != "Kyle") {
		return false;
	}
	return true;
}
```

- Examples
		
```		
Add(2, 4);
  - returns, 6

int sum = Add(2, 4);
  - returns "6" and stores in a variable named 'sum'.
```

```
getName(1); 
returns, "Kyle"

String name = getName(1); 
returns "kyle" and stores in a variable named 'name'.
```

```
getName(2); 
returns, "Invalid ID"

String name2 = getName(2); 
  - returns "Invalid ID" and stores in a variable named 'name'.
```

```
isValidUser(1, "Kyle");
  - returns, "true"

bool isValid = isValidUser(1, "Kyle");
  - returns "true" and stores in a variable named 'isValid'.
```

```
isValidUser(1, "name");
  - returns, "false"

bool isNotValid = isValidUser(1,"name"); 
  - returns "false" and stores in the variable 'isNotValid'.
```


