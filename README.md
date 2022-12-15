# ONE Programming Language

ONE is a general-purpose programming language that is designed to be easy to learn and use. It is a compiled language with a focus on performance and efficiency, while maintaining programmer productivity.

## Features

- **Easy to learn**: ONE is designed to be easy to learn and use. It is a compiled language with a focus on performance and efficiency, while maintaining programmer productivity.
- **Fast**: ONE is a compiled language, which means that it is compiled into machine code before it is executed. It has a couple of optimization phases that make your code optimized and fast.
- **Secure**: ONE has a compiler and you can design your programs without worring about leaking your source code. Your programs will be compiled into machine code before they are executed. This makes it more secure than interpreted languages. If you are going to sell your programs, you can compile them into native executables for any operating system in a single file and share the executable file with your customers. In this way, you can prevent your customers from seeing your source code unlike many other programming languages. such as Python, JavaScript, PHP, and Ruby.
- **Safe**: ONE is a safe language, which means that it is secure to use. It will force you to write secure code. Maybe you do not write secure code, but it will force you to think about security. We tried to force you to follow the best practices and sensible approach to security.
- **Cross-platform**: ONE is designed to be cross-platform, which means that it can be used on any operating system. It is currently supported on Windows, Linux, and macOS. A few of archtechture are supported, such as i386, arm23, and amd64. We will add more archtechture support in the future, But currently, we are focusing on the improvement of the language.
- **Open source**: ONE is open source, which means that it is free to use and modify. It is licensed under the MIT license. We believe that open source is the future of software development. We are trying to extend the open source community and make it more accessible to everyone.
- **Modern**: ONE is a modern language, which means that it has many features that are not found in other languages. It has a built-in package manager, a built-in testing framework, a built-in web server, and many more full-featured libraries for working.
- **Powerful**: ONE has many powerful features that make it a great language for any project. We designed it to be a general-purpose language, which means that it can be used for any project. But we are aware we cannot make it perfect for all projects. So we focused on making it perfect for console softwares and web development. We provide a new novel Web framework called OneWeb.
- **Flexible**: ONE is a flexible language, which means that it is flexible to run on any operating system and different environment with same functionality. We are gathering feedback from the community and we are trying to make it more flexible.
- **Simple**: ONE is a simple language, which means that it is easy to learn and use. It has a clean syntax and follows discipline. We reduced the number of keywords and operators to a minimum, and we made the syntax as simple as possible. It can prevent multi-concept and misunderstanding.
- **Fast**: ONE is a fast language, which means that it is fast to compile and run. It has a very fast compiler in development, and it is very fast to run. It is also very fast to compile and run.
- **Stable**: ONE is not a stable language yet, but we are trying to make it stable. We are trying to make it stable and reliable as soon as possible.
- **Reliable**: ONE is a reliable language, which means that it is reliable to use. By forcing you to write secure code, it will make your programs more reliable. We are tring to add compiler warnings and errors to make it more reliable. It may make it hard for you to write code at first when it's a new language to you, but it will make your code more reliable and secure. So it's better to look at restrictions as a good thing.
- **Scalable**: ONE is going to be a scalable language, we are going to add more features to support concurrency, and safe multi-thread for making it possible for you to extend the scale of your project. As Anna Patterson said the future of programming is cloud. We know it's not possible for big projects to handle big traffic only by scaling up. it's why we are considering scaling out as a big point.
- **Portable**: ONE is a portable language, which means that it is portable to use. It's easy to use on any operating system. End-users can run ONE programs on any operating system without having to install anything. ONE programs can also be compiled into native executables for any operating system in a single file.
- **Efficient**: ONE is an efficient language, which means that it is efficient to use. Reducing memory usage, processors, and developer efforts. We are aware we have to balance between these but we prefer to increase developer efforts to provide a better response in ONE program. ONE is not a language to develop toy software, all we want is to make it easier for you to work on useful, big projects.

There are also many other features that are not listed here.

## Usability space

You can use ONE to create console applications, web applications, and more. You can also use ONE to create libraries and frameworks.

- Console applications
- Web applications
- Libraries
- And more...

We are trying to make ONE a great language for any project. But we are aware we cannot make it perfect for all projects. So we focused on a few fields that we think ONE is perfect for.

## Installation

It is recommended to install ONE using the official installer. You can download the installer from the [official website](https://onelang.org).

### Building from source

If you want to build ONE from source, you can follow the instructions below.

#### Prerequisites

- [Git](https://git-scm.com/downloads)
- [GNU GCC](https://gcc.gnu.org/install/)
- [GNU Make](https://www.gnu.org/software/make/)

#### Building

```bash
git clone https://github.com/One-Language/ONE
cd ONE
make
make install
```

Note: You may need to run `sudo make install` if you are on Linux or macOS and you are not logged in as root.

## Syntax

### Tokens

Tokens are the smallest unit of a program. They are the building blocks of the language. There are many types of tokens in ONE. Here are some of them:

- Keywords
- Values
- Types
- Identifiers
- Operators
- Separators

#### Keywords

Keywords are reserved words in ONE. They have a special meaning and cannot be used as identifiers. Here is a list of keywords in ONE:

| | | |
| ----------- | ------------ | ----------- | ----------- |
| `continue` | `break` | `if` | `else` |
| `for` | `while` | `do` | `switch` |
| `repeat` | `until` | `case` | `default` |
| `return` | `import` | `as` | `enum` |
| `interface` | `try` | `catch` | `throw` |
| `finally` | `defer` | `async` | `await` |
| `func` | `struct` | `union` | `enum` |
| `type` | `typeof` | `is` | `as` |
| `const` | `delete` | | |

### Values

Values are the data that is stored in variables. There are many types of values in ONE. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ------------- |
| `true` | True boolean value | True is a value that represents a true boolean value. |
| `false` | False boolean value | False is a value that represents a false boolean value. |

### Types

Types are the data types of values. There are many types of types in ONE. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `bool` | Boolean | Bool is a type that represents a boolean value. It can be either `true` or `false`. |
| `i8` | Integer 8-bit | Integer 8-bit is a type that represents an integer value. It can be any integer between `-128` and `127`. |
| `i16` | Integer 16-bit | Integer 16-bit is a type that represents an integer value. It can be any integer between `-32768` and `32767`. |
| `i32` | Integer 32-bit | Integer 32-bit is a type that represents an integer value. It can be any integer between `-2147483648` and `2147483647`. |
| `i64` | Integer 64-bit | Integer 64-bit is a type that represents an integer value. It can be any integer between `-9223372036854775808` and `9223372036854775807`. |
| `u8` | Unsigned integer 8-bit | Unsigned integer 8-bit is a type that represents an unsigned integer value. It can be any integer between `0` and `255`. |
| `u16` | Unsigned integer 16-bit | Unsigned integer 16-bit is a type that represents an unsigned integer value. It can be any integer between `0` and `65535`. |
| `u32` | Unsigned integer 32-bit | Unsigned integer 32-bit is a type that represents an unsigned integer value. It can be any integer between `0` and `4294967295`. |
| `u64` | Unsigned integer 64-bit | Unsigned integer 64-bit is a type that represents an unsigned integer value. It can be any integer between `0` and `18446744073709551615`. |
| `f32` | Float 32-bit | Float 32-bit is a type that represents a floating point value. It can be any floating point number between `1.175494351e-38` and `3.402823466e+38`. |
| `f64` | Float 64-bit | Float 64-bit is a type that represents a floating point value. It can be any floating point number between `2.2250738585072014e-308` and `1.7976931348623157e+308`. |
| `char` | Character | Character is a type that represents a character value. It can be any character between `0` and `65535`. Unicode characters are supported. |
| `string` | String | String is a type that represents a string value. It can be any string of characters. |

### Identifiers

Identifiers are the names of variables, functions, classes, etc. They can be any combination of letters, numbers, and underscores. They cannot start with a number. They cannot be a keyword. Here are some examples of identifiers:

| Token | Name | Description |
| -------- | -------- | ----------------------- |

To be completed...

### Operators

Operators are special symbols that perform operations on values. There are many types of operators in ONE. Here are some of them.

There are many types of operators in ONE. Here are some of them:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Logical operators
- Bitwise operators
- Increment and decrement operators
- Ternary operator

#### Arithmetic operators

Arithmetic operators are used to perform arithmetic operations on values. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `+` | Addition | Addition is an operator that adds two values. |
| `-` | Subtraction | Subtraction is an operator that subtracts two values. |
| `*` | Multiplication | Multiplication is an operator that multiplies two values. |
| `/` | Division | Division is an operator that divides two values. |
| `%` | Modulus | Modulus is an operator that returns the remainder of two values. |
| `^` | Exponentiation | Exponentiation is an operator that raises a value to the power of another value. |

#### Assignment operators

Assignment operators are used to assign values to variables. Here are some of them

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `=` | Assignment | Assignment is an operator that assigns a value to a variable. |
| `+=` | Addition assignment | Addition assignment is an operator that adds a value to a variable and assigns the result to the variable. |
| `-=` | Subtraction assignment | Subtraction assignment is an operator that subtracts a value from a variable and assigns the result to the variable. |
| `*=` | Multiplication assignment | Multiplication assignment is an operator that multiplies a value with a variable and assigns the result to the variable. |
| `/=` | Division assignment | Division assignment is an operator that divides a variable by a value and assigns the result to the variable. |
| `%=` | Modulus assignment | Modulus assignment is an operator that returns the remainder of a variable divided by a value and assigns the result to the variable. |
| `^=` | Exponentiation assignment | Exponentiation assignment is an operator that raises a variable to the power of a value and assigns the result to the variable. |

#### Comparison operators

Comparison operators are used to compare two values. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `==` | Equal to | Equal to is an operator that checks if two values are equal. |
| `!=` | Not equal to | Not equal to is an operator that checks if two values are not equal. |
| `>` | Greater than | Greater than is an operator that checks if a value is greater than another value. |
| `<` | Less than | Less than is an operator that checks if a value is less than another value. |
| `>=` | Greater than or equal to | Greater than or equal to is an operator that checks if a value is greater than or equal to another value. |
| `<=` | Less than or equal to | Less than or equal to is an operator that checks if a value is less than or equal to another value. |

#### Logical operators

Logical operators are used to combine two or more conditions. Here are some of them

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `&&` | Logical AND | Logical AND is an operator that checks if two conditions are true. |
| `||` | Logical OR | Logical OR is an operator that checks if one of two conditions is true. |
| `!` | Logical NOT | Logical NOT is an operator that checks if a condition is false. |

#### Bitwise operators

Bitwise operators are used to perform bitwise operations on values. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `&` | Bitwise AND | Bitwise AND is an operator that performs a bitwise AND operation on two values. |
| `|` | Bitwise OR | Bitwise OR is an operator that performs a bitwise OR operation on two values. |
| `^` | Bitwise XOR | Bitwise XOR is an operator that performs a bitwise XOR operation on two values. |
| `~` | Bitwise NOT | Bitwise NOT is an operator that performs a bitwise NOT operation on a value. |
| `<<` | Bitwise left shift | Bitwise left shift is an operator that performs a bitwise left shift operation on a value. |
| `>>` | Bitwise right shift | Bitwise right shift is an operator that performs a bitwise right shift operation on a value. |

#### Increment and decrement operators

Increment and decrement operators are used to increment or decrement a value by 1. Here are some of them:

| Token | Name | Description |
| -------- | -------- | ----------------------- |
| `++` | Increment | Increment is an operator that increments a value by 1. |
| `--` | Decrement | Decrement is an operator that decrements a value by 1. |

#### Ternary operator

This proposal is still under discussion.

### Comments

Comments are used to explain code. They are ignored by the compiler. There are two types of comments in ONE: single-line comments and multi-line comments.

#### Single-line comments

Single-line comments are used to explain a single line of code. They start with `//` and end with a new line. Here is an example:

```c
// This is a single-line comment
```

#### Multi-line comments

Multi-line comments are used to explain multiple lines of code. They start with `/*` and end with `*/`. Here is an example:

```c
/*
This is a multi-line comment
*/
```

### Meanful comments

It's true that comments are ignored by the compiler. But they are not ignored by the programmer. Comments are used to explain code. But sometimes, comments are used to explain the meaning of a value. 

In ONE we have a special type of comments called meanful comments. They are used to explain the meaning of a value. They start with `///` and end with a new line. Here is an example:

```c
/// This is a meanful comment
```

or multiple lines:

```c
/**
* This is a meanful comment
* This is a meanful comment
* This is a meanful comment
*/
```

We will see how to use meanful comments in the future. We will try to have one for each function and variable.

### Types

Types are used to define the data type of a value. There are many types in ONE. Here are some of them:

- `i8` - 8-bit signed integer
- `i16` - 16-bit signed integer
- `i32` - 32-bit signed integer
- `i64` - 64-bit signed integer
- `u8` - 8-bit unsigned integer
- `u16` - 16-bit unsigned integer
- `u32` - 32-bit unsigned integer
- `u64` - 64-bit unsigned integer
- `f32` - 32-bit floating point number
- `f64` - 64-bit floating point number
- `bool` - Boolean value
- `char` - Character
- `string` - String
- `void` - Void

#### Type casting

Type casting is used to convert a value from one type to another. Here is an example:

```c
i32 a = 5;
f32 b = a as f32;
```

#### Type inference

Type inference is used to automatically determine the type of a value. Here is an example:

TODO

### Variables

Variables are used to store values. Here is an example:

```c
i32 a = 5;
```

#### Variable declaration

Variable declaration is used to declare a variable. Here is an example:

```c
i32 a;
```

#### Variable initialization

Variable initialization is used to initialize a variable. Here is an example:

```c
i32 a = 5;
```

#### Variable assignment

Variable assignment is used to assign a value to a variable. Here is an example:

```c
i32 a = 5;
a = 10;
```

#### Variable reassignment

Variable reassignment is used to reassign a value to a variable. Here is an example:

```c
i32 a = 5;
a = 10;
a = 15;
```

### Constants

Constants are used to store values that cannot be changed. Here is an example:

```c
const i32 a = 5;
```

If you try to change the value of a constant, the compiler will throw an error.

Note if you not initialize value for a constant, you will not able to do it later.

Here is an example:

```c
const i32 a;

a = 5; // Error
```

#### Constant declaration


## Contributing

We are always looking for contributors to help us make ONE better. If you are interested in contributing to ONE, please read our [contributing guide](contributing guide.md).

## License

ONE is licensed under the [MIT license](LICENSE).

## Contact

You can contact us via [email](mailto:max@onelang.org) or [Discord](https://discord.gg/xxxxxxxx).

## Credits

All rights reserved to ONE Language Foundation.

