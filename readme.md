# Basic Datatypes and Data Structures in ES6

ES6 has 7 basic datatypes:
<ul>
<li>undefined</li>
<li>Null</li>
<li>Boolean</li>
<li>Number</li>
<li>String</li>
<li>Symbol</li>
<li>Object</li>
</ul>

## The Undefined Datatype:

The Undefined type can have only one value, called <code>undefined</code>. Any variable that does not have any value assigned to it has the value <code>undefined</code>.

### Example 
```javascript
var x;      //creating a variable without any value assigned to it
console.log("the value is", x)     //logs "the value is undefined"
```

## The Null Datatype:

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
