## Operators

 JavaScript has the following types of operators.

 * Arithmetic Operators
 * Assignment Operators
 * Comparison Operators
 * Logical Operators
 * Conditional Operators

**[Operator precedence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence)**

### Arithmetic Operators

 Arithmetic operators are used to perform mathematical operations between numeric operands.

* Addition `+`
* Subtraction `-`
* Multiplication `*`
* Division `/`
* Remainder (MOD) `%`
* Exponentiation `**`
* Increment `++`
* Decrement `--`

```js
let a = 5
let b = 10
let c = 12

console.log(a + b) // 15

console.log(b - a) // 5

console.log(a * b) // 50

console.log(a / b) // 0.5

console.log(a % c) // 5, a remainder of 5 divided by 12

console.log(2 ** 3)  // 8

console.log(a++) // 6

console.log(a--) // 4
```

### Assignment Operators

 An assignment operator assigns a value to its left operand based on the value of its right operand.

 * Assignment `=`
 * Addition assignment `+=`
 * Subtraction assignment `-=`
 * Multiplication assignment `*=`
 * Division assignment `/=`
 * Remainder assignment `%=`
 * Exponentiation assignment `**=`

 ```js
 let x;

  x = 5, y = 10

  x += y; //x would be 15

 x -= 1; //x would be 4

 x *= 5; //x would be 25

 x /= 5; //x would be 1

 x %= 2; //x would be 1

 x **= 2 // x would be 25
   
  
 let sum = 0 

for(let i = 1; i <= 5; i++){
 sum += i
} 
console.log(sum)// 15

for(let i=1; i<= 5 ++i){
 sum+ =i;
}
console.log(sum) // 15


 ```



 ### Comparison Operators

 A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values.

 * Equal `==`
 * Not equal `!=`
 * Strict equal `===`
 * Strict not equal `!==`
 * Greater than `>`
 * Greater than or equal `>=`
 * Less than `<`
 * Less than or equal `<=`

 ```js
 let a = 5;
 let b = 10;
 let c = "5";
 let x = a;

a == c; // returns true

a === c; // returns false

a == x; // returns true

a != b; // returns true

a > b; // returns false

a < b; // returns true

a >= b; // returns false

a <= b; // returns true

a >= c; // returns true

a <= c; // returns true
```


### Logical Operators

* OR `||`
* AND `&&`
* NOT `!`

#### OR (||) Operator

 The “OR” operator is represented with two vertical line symbols:

```js
result = a || b;
```
**OR "||" finds the first truthy value**

In classical programming, the logical OR is meant to manipulate boolean values only. If any of its arguments are true, it returns true, otherwise it returns false.

```js
alert( true || true );   // true
alert( false || true );  // true
alert( true || false );  // true
alert( false || false ); // false
```

* Evaluates operands from left to right.
* For each operand, converts it to boolean. If the result is true, stops and returns the original value of that operand.
* If all operands have been evaluated (i.e. all were false), returns the last operand.

```js
alert( null || 0 || 1 ); // 1 (the first truthy value)

alert( undefined || null || 0 ); // 0 (all falsy, returns the last value)
```


#### AND (&&) Operator

The AND operator is represented with two ampersands &&:

```js
result = a && b;
```

In classical programming, AND returns true if both operands are truthy and false otherwise:

```js
alert( true && true );   // true
alert( false && true );  // false
alert( true && false );  // false
alert( false && false ); // false
```

* Evaluates operands from left to right.
* For each operand, converts it to a boolean. If the result is false, stops and returns the original value of that operand.
* If all operands have been evaluated (i.e. all were truthy), returns the last operand.


#### NOT (!) Operator

The boolean NOT operator is represented with an exclamation sign !.

```js
result = !value;
```

* Converts the operand to boolean type: true/false.
* Returns the inverse value.

```js
alert( !true ); // false

alert( !!"Hello Word!" ); // true
```

### Conditional (ternary) operator

The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition.

```js
condition ? val1 : val2
```

If condition is true, the operator has the value of val1. Otherwise it has the value of val2.

```js
let age = 18

let result = (age >= 18) ? 'adult' : 'small'

alert(result) // adult
```
