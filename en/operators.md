# Operators

An operator in One is a symbol that tells the compiler or interpreter to perform specific mathematical, relational or logical operation and produce final result.

# Example

```
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400)
```

One divides the operators into the following groups:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Logical operators
- Bitwise operators

# Arithmetic operators

| Operator | Name           | Description                            | Example |
| -------- | -------------- | -------------------------------------- | ------- |
| +        | Addition       | Adds together two values               | x + y   |
| -        | Subtraction    | Subtracts one value from another       | x - y   |
| \*       | Multiplication | Multiplies two values                  | x \* y  |
| /        | Division       | Divides one value by another           | x / y   |
| %        | Modulus        | Returns the division remainder         | x % y   |
| ++       | Increment      | Increases the value of a variable by 1 | ++x     |
| --       | Decrement      | Decreases the value of a variable by 1 | --x     |

# Assignment operators

| Operator | Example | Same As    |
| -------- | ------- | ---------- |
| =        | x = 5   | x = 5      |
| +=       | x += 3  | x = x + 3  |
| -=       | x -= 3  | x = x - 3  |
| \*=      | x \*= 3 | x = x \* 3 |
| /=       | x /= 3  | x = x / 3  |
| %=       | x %= 3  | x = x % 3  |
| &=       | x &= 3  | x = x & 3  |
| ^=       | x ^= 3  | x = x ^ 3  |
| >>=      | x >>= 3 | x = x >> 3 |
| <<=      | x <<= 3 | x = x << 3 |

# Comparison operators

| Operator | Name                     | Example |
| -------- | ------------------------ | ------- |
| ==       | Equal to                 | x == y  |
| !=       | Not equal                | x != y  |
| >        | Greater than             | x > y   |
| <        | Less than                | x < y   |
| >=       | Greater than or equal to | x >= y  |
| <=       | Less than or equal to    | x <= y  |

# Logical operators

| Operator | Name        | Description                                             | Example            |
| -------- | ----------- | ------------------------------------------------------- | ------------------ |
| ==       | Logical and | Returns true if both statements are true                | x < 5 && x < 10    |
| \|\|     | Logical or  | Returns true if one or both statements are true         | x < 5 \|\| x < 4   |
| !        | Logical not | Reverse the result, returns false if the result is true | !(x < 5 && x < 10) |
