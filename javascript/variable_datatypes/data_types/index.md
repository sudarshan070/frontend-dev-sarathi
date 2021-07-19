## Data types

**A value in JavaScript is always of a certain type. For example, a string or a number.**

The latest ECMAScript standard defines nine types. Seven data types are primitives and two data types is non-primitive. So the fundamental difference between primitive and non-primitive is that primitive values are immutable and non-primitive values are mutable.
Mutable values are those which can be modified after creation.
Immutable values are those which cannot be modified after creation

**Primitives data types**

* String
* Number
* Bigint
* undefined 
* Boolean
* null 
* Symbol

** non-primitive (Structural Types) ** 

* Object 
* Function

### String

  JavaScript's String type is used to represent textual data. It must be surrounded by quotes.
  In JavaScript, there are 3 types of quotes.

1. Double quotes: "Hello".
2. Single quotes: 'Hello'.
3. Backticks: `Hello`.

Double and single quotes are “simple” quotes. There’s practically no difference between them in JavaScript.

Backticks are “extended functionality” quotes. They allow us to embed variables and expressions into a string by wrapping them in ${…}.

```js
let userName = "Sachin"

console.log(`Hello, ${userName}`) // Hello, Sachin
```

### Number

The number type represents both integer and floating point numbers.
Besides regular numbers, there are so-called “special numeric values” which also belong to this data type: Infinity, -Infinity and NaN

```js
let num = 12
num = 235.5

alert(1 / 0) // Infinity

alert("Hello" / 23) // NaN
```

### BigInt

The BigInt type is a numeric primitive in JavaScript that can represent integers with arbitrary precision.  (The numbers between -(2^53 − 1) and 2^53 − 1.)
A BigInt is created by appending n to the end of an integer or by calling the constructor.


### undefined

A variable that has not been assigned a value has the value undefined.

```js
 let userName;
 alert(userName) // undefined

 let firstName; 
 firstName = undefined
 alert(firstName) // undefined
 ```

 
###  Boolean

Boolean represents a logical entity and can have two values: true and false. 

```js
let isAdmin = false
let isUser = true

let isGreater = 1 > 3 
alert(isGreater) // false
```


## null

The Null type has exactly one value: null. It’s just a special value which represents “nothing”, “empty” or “value unknown”.

```js
let year = null
```

### Object

objects are used to store collections of data and more complex entities.

```js
let obj = {
    name : "Ramesh",
    age: 23
}
```

## The typeof operator

The typeof operator returns the type of the argument.

```js
typeof "Hello" // String
typeof 12 // number
typeof undefined // undefined
typeof true // boolean
typeof 10n // bigint
```
