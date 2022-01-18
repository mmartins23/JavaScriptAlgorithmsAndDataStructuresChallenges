# Iterate Through an Array with a For Loop

A common task in JavaScript is to iterate through the contents of an array. One way to do that is with a for loop. This code will output each element of the array arr to the console:

```js
const arr = [10, 9, 8, 7, 6];

for (let i = 0; i < arr.length; i++) {
   console.log(arr[i]);
}
```

Remember that arrays have zero-based indexing, which means the last index of the array is length - 1. Our condition for this loop is i < arr.length, which stops the loop when i is equal to length. In this case the last iteration is i === 4 i.e. when i becomes equal to arr.length - 1 and outputs 6 to the console. Then i increases to 5, and the loop terminates because i < arr.length is false.

Declare and initialize a variable total to 0. Use a for loop to add the value of each element of the myArr array to total.

### Answer

```js
// Setup
const myArr = [2, 3, 4, 5, 6];
let total = 0;

// Only change code below this line
for (let i = 0; i < myArr.length; i++) {
  total += myArr[i];
}


```

### Code Explanation
* Inititialization: i gets a value of 0 and its used as a counter.

* Condition: the subsequent code is executed as long as i is lower than the length of myArr (which is 5; five numbers but arrays are zero based).

* Final-expression: i is incremented by 1.

* Statement: The function adds myArr[i]'s value to total until the condition isn’t met like so: