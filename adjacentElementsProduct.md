## CodeFights

#### Problem


```javascript 
`Given an array of integers, find the pair of adjacent elements that has the largest product
and return that product. For inputArray = [3, 6, -2, -5, 7, 3], the output should be 
adjacentElementsProduct(inputArray) = 21.`

7 and 3 produce the largest product.

Input/Output
-[time limit] 4000ms (js)
-[input] array.integer inputArray

An array of integers containing at least two elements.

Guaranteed constraints:
2 ≤ inputArray.length ≤ 10,
-1000 ≤ inputArray[i] ≤ 1000.

-[output] integer

The largest product of adjacent elements.
```

#### My Solution

```javascript
function adjacentElementsProduct(inputArray) {
  const newArr = [];
  
  for (let i = 0; i < inputArray.length-1; i++) {
    newArr.push((inputArray[i] * inputArray[i+1]));
   }
  return Math.max.apply(null, newArr);
}
```

#### Thought Process
- I'll have to go through each element and multiply or compare it to the element on either side.
- Loop, forEach, or Map will be needed; I couldn't solve it with forEach or map so just used a for loop.
- Once I have my loop working correctly, I'll need to store the results as an array so I can apply a math function (required research on math functions and application).
- My solution did not work until I realized the 'return' had to be outside the loop.

