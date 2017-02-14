## Arrays
The **array** is one of the most useful and ubiquitous data types in JavaScript. Arrays are simple lists that contain zero or more objects, and can house any data type (even more arrays!). To get an idea of array syntax, let's look first at an _empty_ array.

```js
var list = [];
```

An empty array contains no data and is created here by the empty set of **square brackets** (`[` and `]`). An array with more than zero values would use the same brackets and separate each value with a comma like this:

```js
var numbers = [1, 2, 42, 100];
```

You can mix data types together in a single array:

```js
// numbers and strings
[0.9, "hi!", 56, "there!"]

// even arrays of arrays
[[1,2], [3,4], [5,6]]
```

And you can check the **length** of an array using something called a **property**. Properties are part of **objects** in JavaScript, and objects are a fairly deep topic we won't explore in this tutorial. However, as with most of programming, it's a bit fun to try things before you fully understand how they work. Try running these examples:

```js runnable
// Adding `.length` to the end of array 
console.log([99, 100, 101].length);

// Adding `.length` on to a variable that contains 
// an array works, too. Cool!
var letters = ["a", "b", "c"];
console.log(letters.length);
```

Now you try:
!exercise 48

### Arrays Are Lists
Imagine that you are working on a program and need to store a list of names. We have been given a spreadsheet of names for our program to use. Without using arrays, we could store each item of data individually in our program using a series of variables.

```js
// Without an array, each name might have a unique variable
var a = "Alejandra";
var b = "Jesse";
var c = "Jessica";
var d = "Tamar";
```

Assigning each name to a different variable does what we need it to, but it's cumbersome to work with. Variables need unique names or they will overwrite one another, so every string that we want to store will need its own unique variable.

What if we need to store thousands of names in our program and then do something with all of them, one by one? To access each string we'd need to know the variables that hold every single one of them. If we want the string `"Alejandra"`, we'd have to know about the variable `a`. For `"Jessica"`, we'd have to know it's in `c`. If we wanted to store hundreds of strings, we'd need hundreds of unique variables.

Arrays provide a better way to work with lists. Since arrays *hold lists of data*, all of the names from the above example can be stored in one variable instead of many:

```js
// Each value in an array is separated by a comma
var names = ["Alejandra", "Jesse", "Jessica", "Tamar"];
```

!exercise 18

!exercise 26

In the previous examples, we've looked at arrays that hold only five or six items, but in many programs, arrays might contain hundreds or thousands of items. For now, we'll keep things simple, so you won't be faced with complex data structures. We are just going to scratch the surface of what arrays can do.

### Accessing the Data Stored in an Array
Storing data in arrays is straightforward, but getting data from them can be a little confusing at first. See if you can understand what happens when you run this example:

```js runnable
var students = ["Alejandra", "Jesse", "Jessica", "Tamar"];
console.log(students[3]);
console.log(students[2]);
console.log(students[0]);
```

If the output was confusing, don't worry. Arrays are **zero-indexed**, which means each position in the array has a number, starting with zero on the far left and counting up from there. Part of what makes this confusing is that square brackets are also used to indicate the index you're referring to.

![js-arrayindex.png](https://tiy-learn-content.s3.amazonaws.com/2f957762-js-arrayindex.png)

!exercise 27

!exercise 51

### What's next?
Getting comfortable with arrays and array indexes is an important part of getting starting with JavaScript. The following assessment will give you a few more challenges to make sure you're comfortable with the syntax and concepts. After that, we'll take a brief departure from arrays to introduce the last piece of our puzzle in this mini-course: functions. Once we've covered functions, we'll return to arrays in the final lesson, bringing everything together to build our Mad Libs program.

