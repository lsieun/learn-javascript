# JavaScript Arrays

JavaScript arrays are used to store multiple values in a single variable.

## Creating an Array

Using an array literal is the easiest way to create a JavaScript Array.

Syntax:

```js
var array_name = [item1, item2, ...];
```

Example

```js
var cars = ["Saab", "Volvo", "BMW"];
```

## Converting Arrays to Strings

The JavaScript method `toString()` converts an array to a string of (comma separated) array values.

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.toString();
```

Result

```txt
Banana,Orange,Apple,Mango
```

The `join()` method also joins all array elements into a string.

It behaves just like `toString()`, but in addition you can specify the separator:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");
```

Result

```txt
Banana * Orange * Apple * Mango
```

## Popping and Pushing

When you work with arrays, it is easy to remove elements and add new elements.

This is what **popping** and **pushing** is:

Popping items **out** of an array, or pushing items **into** an array.

### Popping

The `pop()` method removes the last element from an array:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();              // Removes the last element ("Mango") from fruits
```

The `pop()` method returns the value that was "popped out":

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var x = fruits.pop();      // the value of x is "Mango"
```

### Pushing

The `push()` method adds a new element to an array (at the end):

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");       //  Adds a new element ("Kiwi") to fruits
```

The `push()` method returns the new array length:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var x = fruits.push("Kiwi");   //  the value of x is 5
```

## Shifting Elements

Shifting is equivalent to popping, working on the first element instead of the last.

The `shift()` method removes the first array element and "shifts" all other elements to a lower index.

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();            // Removes the first element "Banana" from fruits
```

The `shift()` method returns the string that was "shifted out":

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var x = fruits.shift();    // the value of x is "Banana"
```

The `unshift()` method adds a new element to an array (at the beginning), and "unshifts" older elements:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");    // Adds a new element "Lemon" to fruits
```

The `unshift()` method returns the new array length.

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");    // Returns 5
```

## Changing Elements

Array elements are accessed using their index number:

Array indexes start with `0`. `[0]` is the first array element, `[1]` is the second, `[2]` is the third ...

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[0] = "Kiwi";        // Changes the first element of fruits to "Kiwi"
```

The `length` property provides an easy way to append a new element to an array:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[fruits.length] = "Kiwi";          // Appends "Kiwi" to fruits
```

## Deleting Elements

Since JavaScript arrays are objects, elements can be deleted by using the JavaScript operator `delete`:

Example

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];
delete fruits[0];           // Changes the first element in fruits to undefined
```

Using `delete` may leave undefined holes in the array. Use `pop()` or `shift()` instead.

## Merging (Concatenating) Arrays

The `concat()` method creates a new array by merging (concatenating) existing arrays:

Example (Merging Two Arrays)

```js
var myGirls = ["Cecilie", "Lone"];
var myBoys = ["Emil", "Tobias", "Linus"];
var myChildren = myGirls.concat(myBoys);   // Concatenates (joins) myGirls and myBoys
```

The `concat()` method **does not** change the existing arrays. It always returns **a new array**.

The `concat()` method can take any number of array arguments:

Example (Merging Three Arrays)

```js
var arr1 = ["Cecilie", "Lone"];
var arr2 = ["Emil", "Tobias", "Linus"];
var arr3 = ["Robin", "Morgan"];
var myChildren = arr1.concat(arr2, arr3);   // Concatenates arr1 with arr2 and arr3
```

