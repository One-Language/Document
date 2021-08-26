# For Loop

A for loop is a control flow statement for specifying iteration, which allows code to be executed repeatedly. A for loop has two parts: a header specifying the iteration, and a body which is executed once per iteration. The header often declares an explicit loop counter or loop variable, which allows the body to know which iteration is being executed. For loops are typically used when the number of iterations is known before entering the loop. For loops can be thought of as shorthands for while loops which increment and test a loop variable.

## Syntax

```
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```

- Statement 1 is executed (one time) before the execution of the code block.
- Statement 2 defines the condition for executing the code block.
- Statement 3 is executed (every time) after the code block has been executed.

## Example

```
for (int i = 0; i < 5; i++) {
 cout << i << "\n";
}
```

| :point_up: | The example above will print the numbers 0 to 4. |
| ---------- | :----------------------------------------------- |

**Example explained:**

- Statement 1 sets a variable before the loop starts (int i = 0).

- Statement 2 defines the condition for the loop to run (i must be less than 5). If the condition is true, the loop will start over again, if it is false, the loop will end.

- Statement 3 increases a value (i++) each time the code block in the loop has been executed.
