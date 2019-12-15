# solved-tasks
#### Squares sequence
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
#### Find the next perfect square!
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
#### Formatting decimal places #1
```javascript
function twoDecimalPlaces(number) {
if (number<0) return Math.ceil((number)*100)/100
    else return Math.floor((number)*100)/100
}
```
#### How many times should I go?
```javascript
function howManyTimes(a, i) {
    return Math.ceil(a/i)
}
```
#### Lario and Muigi Pipe Problem
```javascript
function pipeFix(n){
  let j = [];
     for (let i=n[0]; i<=n[n.length-1]; i++){
     j.push(i)
     }
     return j
}
```
#### Calculate Price Excluding VAT
```javascript
function excludingVatPrice(p){
  if (p===null) return -1
  else return +(p/1.15).toFixed(2)
}
```