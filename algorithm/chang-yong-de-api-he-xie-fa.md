# 常用的API和写法

## Array

```
// create array
const arr = new Array("ele1","ele2");
let tmp = arr[0];
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

//for add element
.splice(startIdx,removeEleCount,[eleToBeAdded])
//splice() method returns an array with the deleted items

//
```

### Stack

### Queue

``

### Sort

## Map

## Set

## Constructor

