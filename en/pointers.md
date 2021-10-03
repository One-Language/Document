# Pointers

The pointer in One language is a variable which stores the address of another variable. This variable can be of type int, char, array, function, or any other pointer.

## Declaring a pointer

The pointer in One language can be declared using \* (asterisk symbol). It is also known as indirection pointer used to dereference a pointer.

### Example

```
int *a;//pointer to int
char *c;//pointer to char
```

## Pointer Example

```
string food = "Pizza";  // A food variable of type string
string* ptr = &food;    // A pointer variable, with the name ptr, that stores the address of food

// Output the value of food (Pizza)
cout << food << "\n";

// Output the memory address of food (0x6dfed4)
cout << &food << "\n";

// Output the memory address of food with the pointer (0x6dfed4)
cout << ptr << "\n";
```

## Pointer Example explained

Create a pointer variable with the name ptr, that points to a string variable, by using the asterisk sign _ (string_ ptr). Note that the type of the pointer has to match the type of the variable you're working with.

Use the & operator to store the memory address of the variable called food, and assign it to the pointer.

Now, ptr holds the value of food's memory address.
