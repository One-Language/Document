# Arrays test

An array is used to store a collection of data, but it is often more useful to think of an array as a collection of variables of the same type.

## Create Arrays

To declare an array, define the variable type, specify the name of the array followed by square brackets and specify the number of elements it should store:

```
string colors[4];
```

We have now declared a variable that holds an array of four strings. To insert values to it, we can use an array literal - place the values in a comma-separated list, inside curly braces:

```
string colors[4] = {"Blue", "Red", "Green", "Black"};
```

To create an array of three integers, you could write:

```
int myNum[3] = {10, 20, 30};
```

## Accessing Array Elements

An element is accessed by indexing the array name. This is done by placing the index of the element within square brackets after the name of the array.

### Example

```
string colors[4] = {"Blue", "Red", "Green", "Black"};
cout << colors[0];
// Outputs Blue
```
