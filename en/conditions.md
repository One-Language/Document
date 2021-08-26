# Conditions and If Statements

One supports the usual logical conditions from mathematics:

- Less than: a < b
- Less than or equal to: a <= b
- Greater than: a > b
- Greater than or equal to: a >= b
- Equal to a == b
- Not Equal to: a != b <br>
  You can use these conditions to perform different actions for different decisions.

One has the following conditional statements:

- Use if to specify a block of code to be executed, if a specified condition is true
- Use else to specify a block of code to be executed, if the same condition is false
- Use else if to specify a new condition to test, if the first condition is false
- Use switch to specify many alternative blocks of code to be executed

# The if Statement

The One if statement tests the condition. It executes the if block if condition is true.

## Syntax

```
if(condition){
//code to be executed
}
```

## Example

```
if (20 > 18) {
  System.print("condition is true")
}
```

# The if-else Statement

The One if-else statement also tests the condition. It executes the if block if condition is true otherwise else block is executed.

## Syntax

```
if(condition){
//code if condition is true
}else{
//code if condition is false
}
```

## Example

```
if (20 < 18) {
  System.print("condition is true")
} else {
  System.print("condition is not true")
}

// Outputs "condition is not true"
```

# The else if Statement

The if-else-if ladder statement executes one condition from multiple statements.

## Syntax

```
if(condition1){
//code to be executed if condition1 is true
}else if(condition2){
//code to be executed if condition2 is true
}
else if(condition3){
//code to be executed if condition3 is true
}
...
else{
//code to be executed if all the conditions are false
}
```

## Example

```
if (22 < 10) {
  System.print("a")
} else if (22 < 20) {
  System.print("b")
} else {
  System.print("c")
}
// Outputs "c"
```
