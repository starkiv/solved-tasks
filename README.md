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
#### Parse nice int from char problem
```javascript
function getAge(inputString){
 return parseInt(inputString, 10)
}
```
#### Hex to Decimal
```javascript
function hexToDec(hexString){
  return parseInt(hexString, 16)
}
```
#### Bin to Decimal
```javascript
function binToDec(bin){
return parseInt(bin, 2)
}
```
#### Sum Arrays
```javascript
function sum (n) {
let sum = 0;
    for (let i=0; i<n.length; i++){
    sum+=n[i]
    }
return sum
    
};
```
#### What is type of variable?
```javascript
function type(v) {
  let x = {}.toString.call(v);
  switch (x){
   case '[object Array]': return 'array';
   case '[object Object]': return 'object';
   case '[object String]': return 'string';
   case '[object Number]': return 'number';
   case '[object Date]': return 'date';
   case '[object Null]': return 'null';
   case '[object Undefined]': return 'undefined';
   
   }
}
```
#### Is every value in the array an array?
```javascript
function arrCheck(v){
for (let i = 0; i < v.length; i++){
  if (!Array.isArray(v[i])) return false
}
return true
}
```
#### Enumerable Magic #3 - Does My List Include This?
```javascript
function include(arr, item){
for (let i = 0; i < arr.length; i++){
  if (arr[i] === item) return true
}
return false
}
```
