## CodeFights

#### Problem  

Below we will define an n-interesting polygon. Your task is to find the area of a polygon for a given n.

A 1-interesting polygon is just a square with a side of length 1. An n-interesting polygon is obtained by taking the n - 1-interesting polygon and appending 1-interesting polygons to its rim, side by side. You can see the 1-, 2-, 3- and 4-interesting polygons in the picture below.
```
Example  
For n = 2, the output should be  
shapeArea(n) = 5;  
For n = 3, the output should be  
shapeArea(n) = 13.
Input/Output

[execution time limit] 4 seconds (js)
[input] integer n

Guaranteed constraints:
1 ≤ n < 104.
[output] integer
The area of the n-interesting polygon.
```
Image that was provided in problem:
[shapeArea](https://codefightsuserpics.s3.amazonaws.com/tasks/shapeArea/img/area.png)  

#### My Solution

```javascript
function shapeArea(n) {
  
  return 2*(Math.pow(n, 2)) - (2*n) + 1;
  
}

```

#### Thought Process
- Trying to solve this in a code-thinky kind of way was not working for me so I thought about it as a math problem.
- Using the given information I reverse engineered an algebra equation from it.

