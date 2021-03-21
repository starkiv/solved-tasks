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
#### Pokemon Damage Calculator
```javascript
function calculateDamage(yourType, opponentType, attack, defense){

  if ((yourType === 'fire' && opponentType === 'water') || (yourType === 'grass' && opponentType === 'fire') || (yourType === 'water' && opponentType === 'grass') || (yourType === 'water' && opponentType === 'electric') || (yourType === 'water' && opponentType === 'water') || (yourType === 'electric' && opponentType === 'electric') || (yourType === 'grass' && opponentType === 'grass') || (yourType === 'fire' && opponentType === 'fire')) return Math.ceil(50*(attack/defense)*0.5)
  if ((yourType === 'fire' && opponentType === 'electric') || (yourType === 'grass' && opponentType === 'electric') || (yourType === 'electric' && opponentType === 'fire') || (yourType === 'electric' && opponentType === 'grass')) return Math.ceil(50*(attack/defense)*1)
  if ((yourType === 'fire' && opponentType === 'grass') || (yourType === 'water' && opponentType === 'fire') || (yourType === 'grass' && opponentType === 'water') || (yourType === 'electric' && opponentType === 'water')) return Math.ceil(50*(attack/defense)*2)
  

}
```
#### Decipher this!
```javascript
function decipherThis(str) {
    let newArr = str.split(' ');
    let arr = [];
    for (let i = 0; i < newArr.length; i++){
        let num = newArr[i].replace(/\D/g, '');
        let st = String.fromCharCode(num);
        let code = newArr[i].replace(/\d/g, '');
        arr.push(st + code)
    }
    let f = [];
    for (let i = 0; i < arr.length; i++){
        let string = '';
        if (arr[i].length > 2){
        string += arr[i][0];
        string += arr[i][arr[i].length - 1];
        string += arr[i].slice(2, arr[i].length - 1)
        string += arr[i][1];
        f.push(string);
        } else f.push(arr[i])
    }
    return f.join(' ')
}; 
```
#### Row of the odd triangle
```javascript
function oddRow(n) {
  let num = n ** 2 - (n - 1);
  let arr = [];
  for (let i = 0; i < n; i++){
    arr.push(num + 2 * i)
  } 
  return arr
}
```
#### Pre-FizzBuzz Workout #1
```javascript
function preFizz(n) {
    let arr = [];
    for (let i = 1; i <= n; i++){
        arr.push(i)
    }
    return arr
}
```
#### Training JS #10: loop statement --for
```javascript
function pickIt(arr){
  var odd=[],even=[];
  for (let i = 0; i < arr.length; i++){
      if (arr[i] % 2 === 1) odd.push(arr[i])
      else even.push(arr[i])
  }
  
  
  return [odd,even];
}
```
#### No zeros for heros
```javascript
function noBoringZeros(n) {
  if (n === 0) return 0
  while (n % 10 === 0){
    n = n / 10;
  }
  return n
}
```
#### Beginner Series #3 Sum of Numbers
```javascript
function getSum(a, b){
    let max = Math.max (a, b);
    let min = Math.min (a, b);
    let sum = 0;
    for (let i = min; i <= max; i++){
        sum += i
    }
    return sum
}
```
#### What will be the odd one out?
```javascript
function oddOneOut(str) {
    let obj = {};
    let out = [];
    for (let i = 0; i < str.length; i++){
        if (!obj[str[i]]) obj[str[i]] = 1;
        else delete obj[str[i]];    
}
    for (let i = 0; i < str.length; i++){
        if (obj[str[i]] && str.lastIndexOf(str[i]) === i)
        out.push(str[i]) 
           
}
    return out
}
```
#### Are they the "same"?
```javascript
function comp(array1, array2){
 if (array1 === null || array2 === null) return false
  let arr1 = [...array1];
  let arr2 = [...array2];
  arr1.forEach((num, index) => {
      const matchIndex = arr2.findIndex((num2) => num2 === Math.pow(num, 2))
      if (matchIndex !== -1){
        arr1 = arr1.filter((el, i) => i !== index) 
        arr2 = arr2.filter((el2, i2) => i2 !== matchIndex)
      }
  })

  if (arr2.length === 0) return true
  else return false
}
```
#### Power
```javascript
function numberToPower(number, power){
  if (power === 0) return 1
  let i = 1;
  let j = 0;
  do {
      j++
      i *= number
  } while (j < power)
  return i
}
```
#### Beginner Series #3 Sum of Numbers 2
```javascript
function getSum(a, b){ 
    let max, min; 
    if (a > b) { 
      max = a   
      min = b 
    } else { 
      max = b 
      min = a 
    }  
    let sum = 0; 
    for (let i = min; i <= max; i++){
      sum += i 
    } 
    return sum 
}
```
#### Beginner Series #3 Sum of Numbers 3
```javascript
function getSum(a, b){
    let max = Math.max (a, b);
    let min = Math.min (a, b);
    let sum = 0;
    for (let i = min; i <= max; i++){
        sum += i
    }
    return sum
}
```
#### Tortoise racing
```javascript
function race(v1, v2, g) {
    if (v1 >= v2) return null
    let arr = [];
    let hours = Math.trunc(g / (v2-v1));
    let min = Math.trunc(((g / (v2-v1)) * 60) % 60);
    let sec = Math.trunc(((g / (v2-v1)) * 3600) % 60);
    arr.push(hours, min, sec);
    return arr
}
```
#### Price of Mangoes
```javascript
function mango(q, p){
    let x = q / 3;
    let y = (Math.floor(x) * 2) * p
    return y + (q % 3) * p
}
```
#### Valid Parentheses
```javascript
function validParentheses(parens){
  let count = [0, 0];
  for (let el of parens){
    switch (el){
      case '(': count[0]++
      break;
      case ')': count[1]++
      break;
    }
    if (count[1] > count[0]) return false 
  }
  return count[0] === count[1]
}
```
#### Vasya - Clerk
```javascript
function tickets(peopleInLine){
  let money25 = 0;
  let money50 = 0;
  let money100 = 0;
  for (let i = 0; i < peopleInLine.length; i++){
    if (peopleInLine[i] === 25) money25++
    else if (peopleInLine[i] === 50 && money25 > 0){ 
        money50++
        money25--
        }
    else if (peopleInLine[i] === 100 && money25 > 0 && money50 > 0){ 
        money100++
        money50--
        money25--
        }
    else if (peopleInLine[i] === 100 && money25 > 2){
        money100++
        money25-=3
        } else return 'NO'
  }
  return 'YES'
}
```
#### Drying Potatoes
```javascript
function potatoes(p0, w0, p1) {
    let weightWater = (w0 * p0) / 100;
    let weightDryMatter = w0 - weightWater;
    let newPercentDryMatter = 100 - p1;
    let totalWeight = Math.round(weightDryMatter * 100) / newPercentDryMatter;
    return Math.trunc(totalWeight)
}
```
#### Format data value
```javascript
function formatDataValue(data) {
   if (data < 1000) return `${data}MB`;

   if ((data > 999) && (data < 1000000)){
      let str = data.toString()
      if (str.substring(str.length - 3, str.length) === '000') return `${+str.substring(0, str.length - 3)}GB`
      else return `${+str.substring(0, str.length - 3)}GB ${+str.substring(str.length - 3, str.length)}MB` 
}
  
  if ((data > 999999) && (data < 1000000000)){
      let str = data.toString()

      if (str.substring(str.length - 6, str.length) === '000000') return `${+str.substring(0, str.length - 6)}TB`
      if (str.substring(str.length - 6, str.length) === `${str.substring(str.length - 6, str.length - 3)}000`) return `${+str.substring(0, str.length - 6)}TB ${+str.substring(str.length - 6, str.length - 3)}GB`
      else return `${+str.substring(0, str.length - 6)}TB ${+str.substring(str.length - 6, str.length - 3)}GB ${+str.substring(str.length - 3, str.length)}MB` 
  }
}
```
#### What time is it?
```javascript
let getMilitaryTime = function(input) {
  if ((input.substring(0, input.length - 8) === '12') && (input.substring(input.length - 2, input.length) === 'AM')) return `00:${input.substring(input.length - 7, input.length - 2)}`
  if ((+input.substring(0, input.length - 8) < 12) && (input.substring(input.length - 2, input.length) === 'PM')) return `${+input.substring(0, input.length - 8) + 12}:${input.substring(input.length - 7, input.length - 2)}`
  else return `${input.substring(0, input.length - 2)}`
};
```
#### Unique numbers
```javascript
function uniqueNumbers(numbersArray) {
    let newArr = [];
    for (let i = 0; i < numbersArray.length; i++){
        if (!newArr.includes(numbersArray[i])) newArr.push(numbersArray[i])
    }
    return newArr
}
```
#### Mispelled word
```javascript
function mispelled (word1, word2){
     let count = 0;
     if (word1.length === word2.length){
     for (let i = 0; i < word2.length; i++){
         if (word1.includes(word2[i]) === false) count++
     }
     } 
     if (word1.length > word2.length) { 
         for (let i = 0; i < word1.length; i++){
         if (word2.includes(word1[i]) === false) count++
     }
     }
     if (word1.length < word2.length) { 
         for (let i = 0; i < word2.length; i++){
         if (word1.includes(word2[i]) === false) count++
     }
     }
     if ((word1.length - word2.length > 1) || (word2.length - word1.length > 1)) return false
     if (count <= 1) return true
     else return false
}
```
#### I'm already Tracer
```javascript
function teamComp(heroes) {
  let tank = 0;
  let damage = 0;
  let support = 0;
  for (let i = 0; i < heroes.length; i++){
      if ((heroes[i] === 'D.Va') || (heroes[i] === 'Orisa') || (heroes[i] === 'Reinhardt') || (heroes[i] === 'Roadhog') || (heroes[i] === 'Sigma') || (heroes[i] === 'Winston') || (heroes[i] === 'Wrecking Ball') || (heroes[i] === 'Zarya')) tank++;
      if ((heroes[i] === 'Ashe') || (heroes[i] === 'Bastion') || (heroes[i] === 'Doomfist') || (heroes[i] === 'Genji') || (heroes[i] === 'Hanzo') || (heroes[i] === 'Junkrat') || (heroes[i] === 'McCree') || (heroes[i] === 'Mei') || (heroes[i] === 'Pharah') || (heroes[i] === 'Reaper') || (heroes[i] === 'Soldier: 76') || (heroes[i] === 'Sombra') || (heroes[i] === 'Symmetra') || (heroes[i] === 'Torbjörn') || (heroes[i] === 'Tracer') || (heroes[i] === 'Widowmaker')) damage++;
      if ((heroes[i] === 'Ana') || (heroes[i] === 'Baptiste') || (heroes[i] === 'Brigitte') || (heroes[i] === 'Lúcio') || (heroes[i] === 'Mercy') || (heroes[i] === 'Moira') || (heroes[i] === 'Zenyatta')) support++
  }
  const exstraHeroes = heroes.filter((el, i) => i !== heroes.indexOf(el) && i === heroes.lastIndexOf(el));
  if (exstraHeroes.length > 0) return 'GG'
  const arr = [tank, damage, support];
  if ((tank + damage + support) > 6 || (tank + damage + support) < 6) return 'GG'
  if ((tank === 0) && (damage === 0) && (support === 0)) return 'GG'
  return arr
}
```
#### Expressions Matter
```javascript
function expressionMatter(a, b, c) {
  let x = a * (b + c);
  let y = a * b * c;
  let z = a + b * c;
  let w = (a + b) * c;
  let u = a + b + c;
  return Math.max(x, y, z, w, u)
}
```
#### Binary Addition
```javascript
function addBinary(a,b) {
    
    let x = a + b;
    let y = parseInt(x).toString(2);
    return y
}
```
#### Grasshopper - Messi goals function
```javascript
function goals (laLigaGoals, copaDelReyGoals, championsLeagueGoals) {
  return laLigaGoals + copaDelReyGoals + championsLeagueGoals
}
```
#### Power
```javascript
function numberToPower(number, power){
  if (power === 0) return 1
  let i = 1;
  let j = 0;
  do {
      j++
      i *= number
  } while (j < power)
  return i
}
```
#### Beginner Series #3 Sum of Numbers
```javascript
function getSum(a, b){
    let max = Math.max (a, b);
    let min = Math.min (a, b);
    let sum = 0;
    for (let i = min; i <= max; i++){
        sum += i
    }
    return sum
}
```
#### No zeros for heros
```javascript
function noBoringZeros(n) {
    let str = n + '';
    return +str.replace(/0+$/, '')
}
```
#### Highest and Lowest
```javascript
function highAndLow(numbers){
  let arr = numbers.split(' ');
  arr.sort((a, b) => b - a);
  let str = '';
  str += arr[0] + ' ' + arr[arr.length - 1];
  return str
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
#### Squares sequence
```javascript
function squares(x, n) {
let s = 1;
let arr = [];
for (let i=0; i<n-1; i++){
s*=2
arr.push(Math.pow(x,s))
}
if (n>0) arr.unshift(x)
return arr
}
```
#### Drink about
```javascript
function peopleWithAgeDrink(old) {
   if (old < 14) return "drink toddy"
   if (old < 18 && old > 13) return "drink coke"
   if (old < 21 && old > 17) return "drink beer"
   else if (old > 20) return "drink whisky"
};
```
#### N-th Power
```javascript
function index(array, n){
  if ((array.length <= n)||(array[n] === -1)) return -1
  else
  return Math.pow(array[n], n)
}
```
#### Training JS #29: methods of arrayObject---concat() and join()
```javascript
function bigToSmall(arr){
  const newArr = arr.reduce((t, el) => t.concat(el), []);
  newArr.sort((a, b) => b - a);
  return newArr.join('>')
}
```
#### Sort array by string length
```javascript
function sortByLength (array) {
  return array.sort((a, b) => a.length - b.length)
};
```
#### Row Weights
```javascript
function rowWeights(array){
  const arr = [];
  let count1 = 0, count2 = 0;
  for (let i = 0; i < array.length; i++){
    if (i % 2 === 0) count1 += array[i]
    else count2 += array[i]
  }
    arr.push(count1, count2)
  return arr
}
```
#### Binary to Text (ASCII) Conversion
```javascript
function binaryToString(binary) {
 let n = binary.toString();
 let q = n.replace(/(\d{1,8}(?=(?:\d\d\d\d\d\d\d\d)+(?!\d)))/g, "$1" + ' ');
 let binString = '';

 q.split(' ').map(function(bin) {
    binString += String.fromCharCode(parseInt(bin, 2));
  });
  if (binary === '') return ''
  else return binString;

}
```
#### Grasshopper - Object syntax debug
```javascript
const rooms = {
  first: {
    description: 'This is the first room',
    items: {
      chair: 'The old chair looks comfortable',
      lamp: 'This lamp looks ancient'
      }
  },
  second: {
    description: 'This is the second room',
    items: {
      couch: 'This couch looks like it would hurt your back',
      table: 'On the table there is an unopened bottle of water'
    }
  }
};
```
#### Blood-Alcohol Content
#### Training JS #12: loop statement --for..in and for..of
```javascript
function giveMeFive(obj){
  const arr = [];
  for (let key in obj){
      if (key.length === 5) arr.push(key)
      if (obj[key].length === 5) arr.push(obj[key])
      
  }
  return arr
}
```
#### Ironman Triathlon
```javascript
function iTri(s){
  const triathlon = {};
  
  if (s > 0 && s < 2.5) triathlon['Swim'] = `${(140.6 - s).toFixed(2)} to go!`
  if (s > 2.4 && s < 113) triathlon['Bike'] = `${(140.6 - s).toFixed(2)} to go!`
  if (s > 112 && s < 130.6) triathlon['Run'] = `${(140.6 - s).toFixed(2)} to go!`
  if (s >= 130.6 && s < 140.7) triathlon['Run'] = 'Nearly there!'
  if (s >= 140.7) return 'You\'re done! Stop running!'
  if (s === 0) return 'Starting Line... Good Luck!'
  
  return triathlon
}
```
#### TV channels
```javascript
function redarr(arr) {
  const obj = {};
  const newArr = Array.from(new Set(arr)).sort().map((el, i) => {
      obj[i] = el
  });
  
return obj
}
```
#### Freudian translator
```javascript
function toFreud(string) {
const arr = string.split(' ')
      .map((el) => el = 'sex')
      .join(' ');
if (string === '') return ''
else return arr;
}
```
#### String Reordering
```javascript
function sentence(List) {
  const obj = {};
  for (let i = 0; i < List.length; i++){
      +List[i]
      Object.assign(obj, List[i])
  }
  let newArr = [];
  let arr = Object.entries(obj);
  for (let i = 0; i < arr.length; i++){
    newArr.push([+arr[i][0], arr[i][1]])
  }
  newArr.sort((a, b) => a[0] - b[0]);
  let str = ''
  for (let i = 0; i < newArr.length; i++){
    str += newArr[i][1] + ' '
  }
  return str.trimRight();
}
```
#### Semi-Optional
```javascript
function wrap(value) {
  const wrappedObj = {
    value
  };
  
  return wrappedObj
}
```
#### Total amount of points
```javascript
function points(games) {
let count = 0;
  for (let i = 0; i < games.length; i++){
      if (+games[i][0] > +games[i][2]) count =+ count + 3;
      if (+games[i][0] < +games[i][2]) count =+ count + 0;
      else if (+games[i][0] === +games[i][2]) count++;
  }
  return count
}

```
#### Unique numbers
```javascript
function uniqueNumbers(numbersArray) {
    let newArr = [];
    for (let i = 0; i < numbersArray.length; i++){
        if (!newArr.includes(numbersArray[i])) newArr.push(numbersArray[i])
    }
    return newArr
}
```
#### Split In Parts
```javascript
var splitInParts = function(s, partLength){

  const arr = s.split('');
  const newArr = [];
  const newArr2 = [];
  
  for (let i = 0; i < arr.length; i+=partLength){
      newArr.push(arr.slice(i, i + partLength))
  }  
  
  for (let i = 0; i < newArr.length; i++){
      newArr2.push(newArr[i].join(''))
  }
  
  return newArr2.join(' ')
}
```
#### Training JS #16: Methods of String object--slice(), substring() and substr()
```javascript
function cutIt(arr){
  
  let num = [];
  
  const newArr = arr.map((el, i) => num.push(el.length))
  
  const newArr1 = arr.map((el) => el.slice(0, Math.min(...num)))
  
  return newArr1
  
}
```
#### Number of Decimal Digits
```javascript
function digits(n) {

  const str = '' + n;

  return str.length
}
```

#### Function 3 - multiplying two numbers
```javascript
const multiply = (a, b) => a * b; 
```

#### Nth Root of a Number
```javascript
function root(x, n) {
  return Math.pow (x, 1/n)
}
```

#### Simple Fun #1: Seats in Theater
```javascript
function seatsInTheater(nCols, nRows, col, row) {
  
  const c = (nCols - col) + 1;
  const r = nRows - row;
  return c*r;  
}
```

#### Area of an arrow
```javascript
function arrowArea(a,b) {
  const c = (a ** 2 + b ** 2) ** 0.5;
  const x = c / 2;
  const y = (x + x + a) / 2;
  const s = (y * (y - x) * (y - x) * (y - a)) ** 0.5;
  return +s.toFixed(2);
}
```

#### Who ate the cookie?
```javascript
function cookie(x){
  // ...
  if(typeof x === 'string') return "Who ate the last cookie? It was Zach!"
  else if(typeof x === 'number') return "Who ate the last cookie? It was Monica!"
  else return "Who ate the last cookie? It was the dog!"
  
}
```

#### Is Undefined?
```javascript
function isUndefined(value) {
  return typeof value === 'undefined'? true : false;
}
```

#### Magic bugs
```javascript
function magic(input)
{
  if (typeof input === "undefined")
    return{

        bar: "hello"
    };
  
  else
    return {

        bar: "world"
    };
  
}
```

#### lucky number
```javascript
function isLucky(n) {
  let str = String(n);
  let res = (str.split('')).reduce((el1, el2) => +el1 + +el2);
  if (res % 9 === 0) return true
  else return false
}
```

#### Grasshopper - Debug
```javascript
function weatherInfo (temp) {
  let celsius = (temp - 32) * (5/9);
  if (celsius > 0){
      return celsius + ' is above freezing temperature';
  }else{
      return celsius + ' is freezing temperature';
  }
}
```

#### Debug Basic Calculator
```javascript
var calculate = function calculate(a, o, b) {
 
 if(o === "+")  
   return a + b;
 if(o === "-") 
     return a - b;
 if(o === "/" && b !== 0)  
   return a / b;
 if(o === "*") 
   return a * b;
 else return null;
}
```

#### Grasshopper - Grade book
```javascript
function getGrade (s1, s2, s3) {
  
  const s = (s1 + s2 + s3) / 3; 
  if (s <= 100 && s >= 90) return 'A'
  if (s < 90 && s >= 80) return 'B'
  if (s < 80 && s >= 70) return 'C'
  if (s < 70 && s >= 60) return 'D'
  if (s < 60 && s >= 0) return 'F'

}
```

#### Find the sum of the roots of a quadratic equation
```javascript
function roots(a,b,c){
  let descriminant = b ** 2 - 4 * a * c;
  if (descriminant < 0) return null;
  const x1 = +((-b + descriminant ** 0.5) / (2 * a));
  const x2 = +((-b - descriminant ** 0.5) / (2 * a));
  return +(x1 + x2).toFixed(2)
}
```

#### How old will I be in 2099?
```javascript
function  calculateAge(a, b) {
  if ((a > b) && (a - b !== 1)) return `You will be born in ${a - b} years.`
  if (a === b) return 'You were born this very year!'
  if (b - a === 1) return `You are ${b - a} year old.`
  if (a - b === 1) return `You will be born in ${a - b} year.`
  else return `You are ${b - a} years old.`

}
```

#### Fuel Calculator
```javascript
function fuelPrice(litres, pricePerLitre) {
  if (litres >= 2 && litres < 4) return +((pricePerLitre - 0.05) * litres).toFixed(2)
  if (litres >= 4 && litres < 6) return +((pricePerLitre - 0.1) * litres).toFixed(2)
  if (litres >= 6 && litres < 8) return +((pricePerLitre - 0.15) * litres).toFixed(2)
  if (litres >= 8 && litres < 10) return +((pricePerLitre - 0.20) * litres).toFixed(2)
  if (litres >= 10) return +((pricePerLitre - 0.25) * litres).toFixed(2)
}
```

#### Holiday VI - Shark Pontoon
```javascript
function shark(pontoonDistance, sharkDistance, youSpeed, sharkSpeed, dolphin){
  if (dolphin === true) sharkSpeed = sharkSpeed / 2;
  const yourTime = pontoonDistance / youSpeed;
  const sharkTime = sharkDistance / sharkSpeed;
  if (yourTime < sharkTime) return "Alive!";
  else return "Shark Bait!"
}
```

#### Cat years, Dog years
```javascript
const humanYearsCatYearsDogYears = function(humanYears) {
  let catYears = 24;
  let dogYears = 24;
  if (humanYears === 1){ 
    catYears = 15 
    dogYears = 15 } 
  if (humanYears === 2){
    catYears = 24 
    dogYears = 24
  }
  if (humanYears >= 3){
    for (let i = 3; i <= humanYears; i++){
      catYears += 4
      dogYears += 5
    }  
  }
  
  return [humanYears,catYears,dogYears];
}
```

#### Area or Perimeter
```javascript
const areaOrPerimeter = function(l , w) {
  const area = l * w;
  const perimeter = l * 2 + w * 2;
  if (l === w) return area
  else return perimeter
};
```

#### This is odd
```javascript
function isOdd(n) {
  return Math.abs(n) % 2 === 1 ? true : false
}
```

#### number with 3 roots.
```javascript
function perfectRoots(n){
  const th2 = n ** 0.5;
  const th4 = n ** 0.25;
  const th8 = n ** (1/8);
  if ((th4 === Math.trunc(th4))&&(th2 === Math.trunc(th2))&&(th8 === Math.trunc(th8))) return true
  else return false
}
```


#### Are You Playing Banjo?
```javascript
function areYouPlayingBanjo(name) {
if(name[0]==="R" || name[0]==='r'){
  return name+" plays banjo";
  }
  else{
  return name+" does not play banjo";
}
}
```
#### Plural
```javascript
function plural(n) {
  if (n < 1 || n > 1) {
    return true;
  } else {
    return false;
  }
}
```

#### Cat Years, Dog Years (2)
```javascript
const ownedCatAndDog = function(catYears, dogYears) {
  const arr = [];
  let sum1 = Math.trunc(2 + (catYears - 24) / 4);
  let sum2 = Math.trunc(2 + (dogYears - 24) / 5);
  if (catYears < 15) arr[0] = 0;
  if (dogYears < 15) arr[1] = 0;
  if (catYears === 15 || (catYears < 24 && catYears > 15)) arr[0] = 1;;
  if (dogYears === 15 || (dogYears < 24 && dogYears > 15)) arr[1] = 1;;
  if (catYears === 24) arr[0] = 2;;
  if (dogYears === 24) arr[1] = 2;;
  if (catYears > 24) arr[0] = sum1;
  if (dogYears > 24) arr[1] = sum2;
  return arr
}
```

#### Triangular Treasure
```javascript
function triangular( n ) {
  
  let arr = [];
  
  for (let i = 1; i <= n; i++){
    arr.push(1)
  }
  
  return n > 0 ? arr.map((a, b) => a + b).reduce((a, b) => a + b) : 0
  
}
```
#### Training JS #34: methods of Math---pow() sqrt() and cbrt()
```javascript
function isIntCube(n) {
  return Number.isInteger(Math.cbrt(n));
}

function cutCube(volume, n) {
  return isIntCube(n) && isIntCube(volume / n);
}
```

#### Figurate Numbers #2 - Pronic Number
```javascript
function isPronic(n){
  
  let arr = [];
  
  for (let i = 0; i <= n; i++){
    arr.push(i * (i + 1));
  }
  let result;
  for (let i = 0; i < arr.length; i++){
    if (arr[i] === n) result = arr[i]
  }
  return result === n
}
```

#### Sum of Triangular Numbers
```javascript
function sumTriangularNumbers(n) {
  let res = 0;
  for (let i = 0; i <= n; i++){
    res += i * (i + 1) / 2;
  }
  return res
}
```

#### Basic Calculator
```javascript
function calculate(num1, operation, num2) {

  switch (operation) {
     case '+': return num1 + num2;
     case '-': return num1 - num2;
     case '/': return num2 === 0 ? null : num1 / num2;
     case '*': return num1 * num2;
      default: return null;
 };
}
```

#### Training JS #8: Conditional statement--switch
```javascript
function howManydays(month) {
  switch (month) {
    case 1: return 31;
    case 2: return 28;
    case 3: return 31;
    case 4: return 30;
    case 5: return 31;
    case 6: return 30;
    case 7: return 31;
    case 8: return 31;
    case 9: return 30;
    case 10: return 31;
    case 11: return 30;
    case 12: return 31;    
  }
}
```

#### Money, Money, Money
```javascript
function calculateYears(principal, interest, tax, desired) {
  
    let year = 0;
    let another = desired - principal;
    while (principal < desired){
      principal = principal + (principal * interest) - (principal * interest * tax)
      year++
    }
  return year
}
```

#### Finding Remainder Without Using '%' Operator
```javascript
const remainder = (D, d) =>{
  while (D >= d){
    D = D - d;
  }
  return D;
};
```

#### Multiply the number
```javascript
function multiply(number){
  let str = String(Math.abs(number));
  let count = 0;
  for (let i = 0; i < str.length; i++){
     count++ 
  }
  return number * (5 ** count)
}
```

#### Boiled Eggs
```javascript
function cookingTime(eggs) {
  let count = 0;
  for (let i = 0; i < eggs; i += 8) {
    count += 5
  }
  return count;
}
```

#### Dan's great power generator
```javascript
function danspower(num, power) {
    if (Math.pow(num, power) % 2 === 1) return Math.round(Math.pow(num, power) * 0.1) * 10
    else return Math.pow(num, power)
}
```