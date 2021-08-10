# Basic Datatypes and Data Structures in ES6
<h1> Datatypes</h1>
There were six basic datatypes that were available to users with ES5:

- [undefined](#the-undefined-datatype)
- [Null](#the-null-datatype)
- [Boolean](#boolean)
- [Number](#number)
- [String](#string)
- [Object](#object)


After the introduction of ES6 a new datatype has been added to the list of datatypes that were previously available.

- [Symbol](#symbol)

### The Undefined Datatype:

The Undefined type can have only one value, called <code>undefined</code>. Any variable that does not have any value assigned to it has the value <code>undefined</code>.

### Example 
```javascript
var x;      //creating a variable without any value assigned to it
console.log("the value is", x)     //logs "the value is undefined"
```

### The Null Datatype:

The Null type can have exactly one value, called <code>null</code>. A null value represents a reference that points, generally intentionally, to a nonexistent or invalid object or address.

### Example
```javascript
let obj = null;
console.log(typeof obj); // object
```

## The Boolean Type:

The Boolean type is a logical datatype that can have only two values <code>true</code> or <code>false</code>. For example, in JavaScript, Boolean conditions are used to decide whether a section of code is to be executed (if statements) or to be repeated (for loops).

### Example
```javascript
if(boolean condition){
    //code to be executed if condition is true.
}
```
## The Number Type:

The Number type represents both, <code>integers</code> and <code>floating-point</code> numbers in JavaScript. JavaScript uses the  <a href="https://en.wikipedia.org/wiki/IEEE_floating_point">IEEE-754 format</a> to represent them.

### Example
```javascript
let num = 100;  //integer   
let f1 = 12.5;  //floating point
```

## The String Type:

The String type is a sequence of zero or more characters. A literal string can begin with single quote <code>(')</code> or double quote <code>(")</code>. If a string begins with single quote it must end with a single quote and if a string begins with double quote it must end with a double quote.

### Example 
```javascript
let hello = 'Hi';
let s = "It's a valid string";
let str = 'I\'m also a string'; // use \ to escape the single quote (')
```

## The Object Type:

The Object type is a collection of properties, where each property is defined as a key-value pair.

### Example
```javascript
let emptyObject = {}; // Empty object
let person = {          // object having two properties
    firstName: 'John',
    lastName: 'Doe'
};
```

## The Symbol Type:

The Symbol type is only available with ES6. Symbol is the set of all non-String values that may be used as the key of an Object property. Each Symbol value is unique and immutable and holds an associated value called [Description] that is either undefined or a String value. A symbol value is created by invoking the <code>symbol</code> function.

### Example
```javascript
let Sym1 = Symbol("Sym")
let Sym2 = Symbol("Sym")

console.log(Sym1 === Sym2) // returns "false" because Symbols are guaranteed to be unique.
```

<h1>Data Structures</h1>

## Before ES6 following six basic data structures were available in ES5:

## Arrays

An array is a collection of items of any data type. JavaScript array is expandable and items can be added as they come without worrying about its size.

### Example
```javascript
let myArray = [];                //assign values later
let myArray = [3,2,5,0,1,7];    //Using Array class constructor.
let myArray = new Array(3,2,5,0,1,7);
```

## Linked Lists

Linked lists uses a referencing system unlike the indexing system used in the arrays to store the information. Elements are stored in nodes that also contain a pointer to the next node which repeates until all the nodes are linked.

### Example
```javascript  
// User defined class node
class Node {
	// constructor
	constructor(element)
	{
		this.element = element;
		this.next = null
	}
}
```

## Stacks

Stack is a linear data structure in which addition or removal of element follows a particular order i.e. LIFO(Last in First Out) AND FILO(First in Last Out). Functions that can be implemented are: <code>push(), pop(), peek(), isEmpty(), printStack()</code>

### Example
```javascript           
// Stack class
class Stack {

	// Array is used to implement stack
	constructor()
	{
		this.items = [];
	}
}
```

## Queues

A Queue works on the FIFO(First in First Out) principle. Hence, it performs two basic operations that is addition of elements at the end of the queue and removal of elements from the front of the queue. Functions that can be performed on a queue are: <code>enqueue(), dequeue(), front(), isEmpty(), printQueue()</code>

### Example
```javascript
// Queue class
class Queue
{
	// Array is used to implement a Queue
	constructor()
	{
		this.items = [];
	}
}
```

## Trees

A tree is basically a linked list keeping the references of many child nodes in a hierarchical model. Each node can have no more than one parent. 

### Example
```javascript
class TreeNode {
  constructor(value) {
    this.value = value;
    this.descendants = [];
  }
}
```

## Graphs
A graph is a non-linear data structure where a node can have zero or more adjacent elements.The connection between two nodes is called edge. Nodes can also be called vertices. Graphs are divided into two categories: <code>Directed and Undirected</code>

### Example
```javascript
// create a graph class
class Graph {
	// defining vertex array and
	// adjacent list
	constructor(noOfVertices)
	{
		this.noOfVertices = noOfVertices;
		this.AdjList = new Map();
	}
}
```
## ES6 has introduced two new data structures to JavaScript called <code>maps</code> and <code>sets</code>:

## Maps

The Map object is a simple key/value pair. Keys and values in a map may be primitive or objects.

### Example
```javascript
var map = new Map(); 
map.set('name','Mountblue'); 
map.get('name'); // Mountblue
```

## Sets

The sets are similar to an array data structure with an exception that it cannot contain duplicate values and values can only be unique.

###  Example
```javascript
var set1 = new Set(["sumit","sumit","amit","anil","anish"]); // contains ["sumit","amit","anil","anish"]
var set2 = new Set("fooooooood");   // contains 'f', 'o', 'd'
var set3 = new Set([10, 20, 30, 30, 40, 40]);   // contains [10, 20, 30, 40]
var set4 = new Set();    //it is an empty set
```

# New features available with ES6


## Reference links:
<ul><li>Geeksforgeeks.com</li>
<li>https://medium.com/siliconwat/data-structures-in-javascript-1b9aed0ea17c</li>
<li>https://262.ecma-international.org/6.0/#sec-ecmascript-data-types-and-values</li>
<li>https://www.tutorialspoint.com/es6/es6_collections.htm</li>
<li>https://www.javascripttutorial.net/javascript-data-types</li>
<li>https://developers.decoded.africa/index.php/2020/08/03/es6-javascript-data-structures-you-should-know/</li></ul>
