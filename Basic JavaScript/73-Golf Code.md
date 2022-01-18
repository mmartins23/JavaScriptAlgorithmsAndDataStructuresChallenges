# Golf Code

In the game of golf, each hole has a par, meaning, the average number of strokes a golfer is expected to make in order to sink the ball in the hole to complete the play. Depending on how far above or below par your strokes are, there is a different nickname.

Your function will be passed par and strokes arguments. Return the correct string according to this table which lists the strokes in order of priority; top (highest) to bottom (lowest):

Strokes	Return
```js
1	"Hole-in-one!"
<= par - 2	"Eagle"
par - 1	"Birdie"
par	"Par"
par + 1	"Bogey"
par + 2	"Double Bogey"
>= par + 3	"Go Home!"
```

par and strokes will always be numeric and positive. We have added an array of all the names for your convenience.


### Answer

```js
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
    // Only change code below this line
    if (1 == strokes) return names[0];
    else if (par -2 >= strokes) return names[1];
    else if (par -1 === strokes) return names[2];  
    else if (par === strokes) return names[3];
    else if (par + 1 === strokes) return names[4];
    else if (par + 2 === strokes) return names[5];
    else if (par + 3 <= strokes) return names[6];
    // Only change code above this line
}
  // Change these values to test
  golfScore(5, 1);
  ```


### Code Explanation
Since we already have an array defined in the variable names we can take advantage of it and use it for our return statements using indexes (eg: names[0] is the first one). 

That way, if you ever need to change a specific result you wouldn’t need to look for it inside the function, it’d be at the beginning, in your array.