# Using Objects for Lookups

Objects can be thought of as a key/value storage, like a dictionary. If you have tabular data, you can use an object to lookup values rather than a switch statement or an if/else chain. This is most useful when you know that your input data is limited to a certain range.

Here is an example of a simple reverse alphabet lookup:

```js
const alpha = {
  1:"Z",
  2:"Y",
  3:"X",
  4:"W",
  ...
  24:"C",
  25:"B",
  26:"A"
};

alpha[2];
alpha[24];

const value = 2;
alpha[value];

```

```
alpha[2] is the string Y, alpha[24] is the string C, and alpha[value] is the string Y.
```

Convert the switch statement into an object called lookup. Use it to look up val and assign the associated string to the result variable.



### Answer

```js
// Setup
function phoneticLookup(val) {
  var result = "";

  // Only change code below this line
  var lookup={
    "alpha":"Adams",
    "bravo":"Boston",
    "charlie":"Chicago",
    "delta":"Denver",
    "echo":"Easy",
    "foxtrot":"Frank"
  };
  
  result = lookup[val];

  // Only change code above this line
  return result;
}

// Change this value to test
phoneticLookup("delta");
```


### Code Explanation
This is what happens

You calll the function phoneticLookup and pass the value of “charlie”

The function has the object array “Lookup” inside to figure out what to output (“Chicago”)

Inside the function, you store the result by searching through that object array “Lookup” by passing it an input of “Charlie” to output “Chicago”
Return the value