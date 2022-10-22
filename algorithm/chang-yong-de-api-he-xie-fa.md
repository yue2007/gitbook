# 常用的API和写法

## Array

```
// create array
const arr = new Array("ele1","ele2");
let tmp = arr[0];

//create 2d array m*n and fill with -1 
const arr = new Array(m).fill().map(() => new Array(n).fill(-1));
```

typeof Array is object\
Objects use **names** to access its "members". In this example, `person.firstName` returns John:\
`const person = {firstName:"John", lastName:"Doe", age:46};`

### How to check an array

```
// method 1: typeof
let type = typeof arr; //type is object

//method 2: Array.isArray()
Array.isArray(arr);

//method 3:instanceof 
arr instanceof Array;
```

### Array prototype

### String

```
//String
.toString(); //(comma separated)
.join();

//Stack
.push();
.pop();

//Queue
//remove first element //return the element value
.shift();
//add element to the beggining of the array //return new array
.unshift();

//delete, leaves undefined holes in the array.
const fruits = ["Banana", "Orange", "Apple", "Mango"];
delete fruits[0];

//Merging
//concat() does not change the existing arrays.

//for add element //change the original array
.splice(startIdx,removeEleCount,[eleToBeAdded])
//splice() method returns an array with the deleted items

//create a new array but not change the original array
//rest of the array
.slice(agr1); 

//start from arg1 to arg2 but not iclueded arg2
.slice(arg1,arg2);
```

### Stack

<pre><code><strong>//first in first out
</strong><strong>.pop()
</strong>.push()

.size()</code></pre>

### Queue

```
//first in
const array1 = [1, 2, 3];
console.log(array1.unshift(4, 5));
console.log(array1);  // expected output: Array [4, 5, 1, 2, 3]

//last out
const array1 = [1, 2, 3];
const firstElement = array1.shift();
console.log(array1);  // expected output: Array [2, 3]
```

``

### Sort

```
//built in sort 
//sort by beginning number or Alphabet
const array1 = [1, 30, 4, 21, 100000];
array1.sort();
console.log(array1); // expected output: Array [1, 100000, 21, 30, 4]

//sort by number // acceding order
arr.sort((a,b) => a - b);
```

## Map



```
// Some code
const map = new Map();
.set();
.get();
.delete(key);
.has();
```

## Set

## Constructor

