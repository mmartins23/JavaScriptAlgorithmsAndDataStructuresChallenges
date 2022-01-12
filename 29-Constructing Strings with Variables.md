# Constructing Strings with Variables
Sometimes you will need to build a string, Mad Libs style. By using the concatenation operator (+), you can insert one or more variables into a string you're building.

Example:

```js
const ourName = "freeCodeCamp";
const ourStr = "Hello, our name is " + ourName + ", how are you?";
```

ourStr would have a value of the string Hello, our name is freeCodeCamp, how are you?.

Set myName to a string equal to your name and build myStr with myName between the strings My name is and and I am well!


### Answer

```js
// Only change code below this line
const myName = "Peter Parker";
const myStr = "Spider-Man is:" + myName + ".";
```
