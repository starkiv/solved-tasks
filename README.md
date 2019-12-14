# solved-tasks
* task 1
```javascript
const a = 123;
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