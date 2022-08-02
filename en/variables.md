# Variables

Variables are used to store information to be referenced and manipulated in a computer program. They also provide a way of labeling data with a descriptive name, so our programs can be understood more clearly by the reader and ourselves. It is helpful to think of variables as containers that hold information. Their sole purpose is to label and store data in memory. This data can then be used throughout your program.

# Declaring (Creating) Variables

```
type variable = value;
```

Where type is one of One's types (such as int or string), and variable is the name of the variable (such as x or name). The equal sign is used to assign values to the variable.

## Example

```
string text = "One is awesome!"
System.print(text)
```

Note that if you assign a new value to an existing variable, it will overwrite the previous value:

## Example

```
string text = "One is awesome!"
text = "One is cool :)"
System.print(text) //the output will be: One is cool :)
```

# Other types

In One, there are different types of variables, for example:

## Example

```
int number = 10;
float floatNumber = 10.99f;
char letter = 'O';
boolean bool = true;
string text = "One is awesome!";
```

# Declare Many Variables

To declare more than one variable of the same type, use a comma-separated list:

## Example

```
int a = 10, b = 15, c = 20
System.print(a)
System.print(b)
System.print(c)
```
