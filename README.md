# solved-tasks
####Squares sequence
```javascript
function squares(x, n){
  let s = 1;
  let arr = [];
  for (let i=0; i<n-1; i++){
    s*=2
    arr.push (Math.pow(x,s))
  }
  if (n>0) arr.unshift(x)
  return arr
}
```
####Find the next perfect square!
```javascript
function findNextSquare(sq){
 let arr =[];
 for (let i=sq; i<sq+700000; i++){
   if (Number.isInteger(Math.sqrt(i)) === true) arr.push(i)  
   }
 if ((Number.isInteger(Math.sqrt(sq)) === false)) return -1
   else return arr[1] 
}
```