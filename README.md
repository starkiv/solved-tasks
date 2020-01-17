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
#### How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
let sum = 0;  
for (let i = 0; i < classPoints.length; i++){  
  sum = sum + classPoints[i]; 
}
let p = sum/classPoints.length;
if(p<=yourPoints) return true
if(p>yourPoints) return false
}
```
#### Difference of Volumes of Cuboids
```javascript
function findDifference(a, b) {
let a1=1;
let b1=1;
  for (let i = 0; i < a.length; i++){
  a1*=a[i]
  }
  for (let i = 0; i < b.length; i++){
  b1*=b[i]
  }
  return Math.abs(b1-a1)
}
```
#### Total amount of points
```javascript
function points(games) {
let sum = 0;
  for (let i=0; i<games.length; i++){
     if (games[i][0] > games[i][2]) sum+=3
     else if (games[i][2] > games[i][0]) sum+=0
     else if (games[i][0] === games[i][2]) sum+=1
  }
  return sum
}
```
#### How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
let sum = 0;  
for (let i = 0; i < classPoints.length; i++){  
  sum = sum + classPoints[i]; 
}
let p = sum/classPoints.length;
if(p<=yourPoints) return true
if(p>yourPoints) return false
}
```
#### Calculate average
```javascript
function find_average(a) {
let a1=0;
let b=0;
  for (let i = 0; i < a.length; i++){
  a1++
  b+=a[i]
  }
  return Math.abs(b/a1)
}
```
#### Count of positives / sum of negatives
```javascript
function countPositivesSumNegatives(input) {
let c = 0;
let sum = 0;
let arr = [];
if (!input || !input.length) return []
for (let i=0; i<input.length; i++){
        if (input[i]>0) sum++
        if (input[i]<0) c+=input[i]
    }
arr.push(sum)
arr.push(c) 
return arr

}
```
#### Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
let v = [];
let sum = 0;
for (let i=0; i<arr.length; i++){
    if (arr[i] === Math.trunc(arr[i])) v.push(arr[i]**3)
    else if (typeof(arr[i]) === 'string') return undefined
}
for (let i=0; i<v.length; i++){
    if ((v[i]%2===1)||(v[i]%2===-1)) sum+=v[i]
}
return sum
}
```
#### Remove the minimum
```javascript
function removeSmallest(n) {
let arr=[];
let e=Math.min(...n);
let r=n.indexOf(e)
    for (let i=0; i<n.length; i++){
        if (i !== r) arr.push(n[i])
    }
return arr

}
```
#### Find Maximum and Minimum Values of a List
```javascript
var min = function(list){
    
    return Math.min(...list);
}

var max = function(list){
    
    return Math.max(...list);
}
```
#### Sum without highest and lowest number
```javascript
function sumArray(array) {
let sum = 0;
if (!array || array.length<2) return 0
for (let i=0; i<array.length; i++){
  sum+=array[i]
}
return sum - Math.min(...array) - Math.max(...array)
}
```
#### Find the divisors!
```javascript
function divisors(integer) {
let arr = [];

  for (let i=2; i<integer; i++){
    if (integer%i === 0)
      arr.push(i)
  }
  if (arr.length === 0) return `${integer} is prime`
  else return arr
};
```
#### Count by X
```javascript
function countBy(x, n) {
  let z = [];
for (let i=1; i<=n*x; i++){
    if (i%x === 0) z.push(i)
}
  return z;
}
```
#### Unfinished Loop - Bug Fixing #1
```javascript
function createArray(number){
  let newArray = [];
  
  for(let counter = 1; counter <= number; counter++){
    newArray.push(counter);
  }
  
  return newArray;
}
```
#### Reversed sequence
```javascript
const reverseSeq = n => {
let arr = [];
for (let i=n; i>0; i--){
    arr.push(i)
}
  return arr;
};
```
#### Training JS #4: Basic data types--Array
```javascript
function getLength(arr){
  return arr.length
}
function getFirst(arr){
  return arr[0]
}
function getLast(arr){
  return arr[arr.length-1]
}
function pushElement(arr){
  var el=1;
  arr.push(el)
  return arr
}
function popElement(arr){
  arr.pop() 
  return arr
}
```
#### You only need one - Beginner
```javascript
function check(a, x) {
  return a.includes(x)
}
```
#### Be Concise IV - Index of an element in an array
```javascript
function find(a,e){
if(a.indexOf(e)==-1) return "Not found"
else return a.indexOf(e)}
```
#### JavaScript Array Filter
```javascript
function getEvenNumbers(nA){
 function nArr (Even){
    if (Even%2 === 0) return Even
 }

const arr = nA.filter(nArr)
return arr
}
```
#### Array.diff
```javascript
function array_diff(a, b) {
  let arr = [];
    for (let i=0; i<a.length; i++){
      if (!b.includes(a[i])) arr.push(a[i])
    }
  return arr  
}
```
#### Removing Elements
```javascript
function removeEveryOther(arr){
 const rem = arr.filter((el, i) => i%2===0)
 return rem
}
```
#### filterEvenLengthWords
```javascript
function filterEvenLengthWords(words) {
function getWord(word) {
  if (word.length % 2 === 0) return word;
}
const arr2 = words.filter(getWord);
return arr2
}
```
#### Find Duplicates
```javascript
function duplicates(arr) {
  const arr2 = arr.filter ((el, i) => i !== arr.indexOf(el) && i == arr.lastIndexOf(el));
  return arr2
}
```
#### Train to remove duplicates from an array with filter()
```javascript
function unique(arr) {
const v = arr.filter ((el, i) => i === arr.indexOf(el))
return v

}
```
#### Jenny's secret message
```javascript
function greet(name){
  if(name !== "Johnny") return "Hello, " + name + "!"
   else return "Hello, my love!";
}
```
#### If you can't sleep, just count sheep!!
```javascript
var countSheep = function (num){
let a = '';
  for (let i=1; i<=num; i++){
    a += `${i} sheep...`
  }
  return a
}
```
#### Numbers to Letters
```javascript
function switcher(x){
let arr2 = [];
let arr = ['z','y','x','w','v','u','t','s','r','q','p','o','n','m','l','k','j','i','h','g','f','e','d','c','b','a','!','?',' '];
for (let i=0; i<x.length; i++){
   for (let j=0; j<arr.length; j++){
     if (x[i]==j+1) arr2.push(arr[j])
   }
}
return arr2.join('')
}
```
#### Unique In Order
```javascript
var uniqueInOrder=function(it){
let arr = [];
let arr2 = [];
  for (let i=0; i<it.length; i++){
    arr.push(it[i])
  }
  for  (let i=0; i<arr.length; i++){
    if (arr[i]!==arr[i-1]) arr2.push(arr[i])
  }
return arr2  
}
```
#### Triple Trouble
```javascript
function tripleTrouble(one, two, three){
let str='';
  for (let i=0; i<one.length; i++){
     str+=one[i]+two[i]+three[i]
  }
  return str
 }
```
#### Spacify
```javascript
function spacify(str) {
let str2='';
  for (let i=0; i<str.length-1; i++){
     str2+=str[i]+' ';
  } 
  return str2+str[str.length-1]
}
```
#### Find the capitals
```javascript
var capitals = function (w) {
let arr = [];
	for (let i=0; i<w.length; i++){
    if (w[i].toUpperCase() === w[i]) arr.push(i)
  }
  return arr
};
```
#### repeatIt
```javascript
var repeatIt = function(str, n) {
  if (typeof str === 'string'){ return str.repeat(n)
  }else {
    return 'Not a string'}
  }
```
#### Don't give me five!
```javascript
function dontGiveMeFive(start, end){
  let arr = [];
  for(let i = start; i <= end; i++){
    let j = i+'';
    if (j.includes('5') === false) arr.push(i)
  }
  return arr.length
}
```
#### Credit Card Mask
```javascript
function maskify(cc) {
let a = '#';
let b = '';
if(cc.length > 4) b += a.repeat(cc.length-4)
else b = '';
return b + cc.slice(-4)
}
```
#### Tail Swap
```javascript
function tailSwap(arr) {
  let arr2 = [];
  for(let i = 0; i < arr.length; i++){
    arr2.push(arr[i].slice(0, arr[i].indexOf(':')+1))
  }
  arr2[0] += arr[1].slice(arr[1].indexOf(':')+1)
  arr2[1] += arr[0].slice(arr[0].indexOf(':')+1)
  return arr2
}
```
#### Duck Duck Goose
```javascript
function duckDuckGoose(p, g) {
let str = '';
  for(let i = 0; i <= g; i++){
     if(i+1 === g) str += p[i].name
     if(i+1 >= p.length){
     g-=p.length;
     i=0
     }
  }
//   console.log(str)
   return str
 
  
  
}
```
#### Welcome!
```javascript
function greet(language) {
	 let hi = {
     english: 'Welcome',
     czech: 'Vitejte',
     danish: 'Velkomst',
     dutch: 'Welkom',
     estonian: 'Tere tulemast',
     finnish: 'Tervetuloa',
     flemish: 'Welgekomen',
     french: 'Bienvenue',
     german: 'Willkommen',
     irish: 'Failte',
     italian: 'Benvenuto',
     latvian: 'Gaidits',
     lithuanian: 'Laukiamas',
     polish: 'Witamy',
     spanish: 'Bienvenido',
     swedish: 'Valkommen',
     welsh: 'Croeso',
     IP_ADDRESS_INVALID: 'Welcome',
     IP_ADDRESS_NOT_FOUND: 'Welcome', 
     IP_ADDRESS_REQUIRED: 'Welcome',
   }
   return hi[language]
}
```
#### Make a function that does arithmetic!
```javascript
function arithmetic(a, b, operator){
  if (operator === 'add') return a + b
  if (operator === 'subtract') return a - b
  if (operator === 'multiply') return a * b
  if (operator === 'divide') return a / b
}
```
#### Numbers to Objects
```javascript
function numObj(s){
  const arr = [];
  s.map(v => arr.push(String.fromCharCode(v)))
  const obj = Array.from({length:s.length}, x => x = {});
  obj.map((v, i) => v[s[i]] = arr[i])
  return obj
}
```
#### Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages
```javascript
function countLanguages(list) {
let counter = list.reduce(function (o, i) {
  if (!o.hasOwnProperty(i.language)) {
    o[i.language] = 0;
  }
  o[i.language]++;
  return o;
}, {});

return counter
}
```
#### Most valuable character
```javascript
function solve(st) {
   let max = 0, result = [], div;
   for (let k of st){
      div = st.lastIndexOf(k) - st.indexOf(k);
      if (max < div) max = div;
   }
   for (let k of st){
      div = st.lastIndexOf(k) - st.indexOf(k);
      if (max === div) result.push(k);
   }
   return result.sort()[0]
}
```
#### Permute a Palindrome
```javascript
function permuteAPalindrome (input) { 
 let count = 0;
  const dict = input.split('').reduce((acc, curr) => ((acc[curr] = acc[curr] ? acc[curr] + 1 : 1), acc),
    {}
  );
  for (let i in dict) {
    if (dict[i] % 2 !== 0) {
      count++;
    }
    if (count === 2) return false;
  }
  return true;
}
```
#### How many days are we represented in a foreign country?
```javascript
function daysRepresented(trips){
   let hours = {};
   for (let i = 0; i < trips.length; i++){
      for (let j = trips[i][0]; j <= trips[i][1]; j++){
         hours[j] = 1;
      }
   }
   let result = 0;
   for (key in hours){
   result += hours[key]
   }
   return result
}
```
#### The Office II - Boredom Score
```javascript
function boredom(staff){
  let arr = Object.entries(staff);
  let nArr = [];
  for (let i = 0; i < arr.length; i++){
    if (arr[i][1] === 'accounts') nArr.push(1)
    if (arr[i][1] === 'finance') nArr.push(2)
    if (arr[i][1] === 'canteen') nArr.push(10)
    if (arr[i][1] === 'regulation') nArr.push(3)
    if (arr[i][1] === 'trading') nArr.push(6)
    if (arr[i][1] === 'change') nArr.push(6)
    if (arr[i][1] === 'IS') nArr.push(8)
    if (arr[i][1] === 'retail') nArr.push(5)
    if (arr[i][1] === 'cleaning') nArr.push(4)
    if (arr[i][1] === 'pissing about') nArr.push(25)
    }
  const result = nArr.reduce((k, v) => k + v, 0)
  if (result <= 80) return 'kill me now'
  if ((result > 80) && (result < 100)) return 'i can handle this'
  else return  'party time!!'
}
```
#### Miles per gallon to kilometers per liter
```javascript
function converter (mpg) {
  let a = mpg / 4.54609188;
  let b = a * 1.609344;
  return +b.toFixed(2)
}
```
#### Find the Slope
```javascript
function slope(points){
   let result = (points[3] - points[1])/(points[2] - points[0])
   if ((points[2] - points[0]) === 0) return 'undefined' 
   else return result.toFixed()
}
```
#### simple calculator
```javascript
function calculator(a,b,sign){
   if (typeof a !== 'number' || typeof b !== 'number') return 'unknown value'
   else
   switch (sign) {
     case '+':  
     return a + b
     break
     case '*':
     return a * b
     break
     case '/':
     return a / b
     break
     case '-':
     return a - b
     break
     default: 
     return 'unknown value' 
   }

}
```
#### Training JS #7: if..else and ternary operator
```javascript
function saleHotdogs(n){
  if (n < 5) return n * 100
  if (n >= 5 && n < 10) return n * 95
  else return n * 90
}
```
#### Get Planet Name By ID
```javascript
function getPlanetName(id){
  let name;
  switch(id){
    case 1:
      name = 'Mercury'
      break
    case 2:
      name = 'Venus'
      break
    case 3:
      name = 'Earth'
      break
    case 4:
      name = 'Mars'
      break
    case 5:
      name = 'Jupiter'
      break
    case 6:
      name = 'Saturn'
      break
    case 7:
      name = 'Uranus'
      break
    case 8:
      name = 'Neptune'
  }
  
  return name;
}
```