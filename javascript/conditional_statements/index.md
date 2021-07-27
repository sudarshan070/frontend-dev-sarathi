# Conditional Statements

**JavaScript statements are the commands to tell the browser to what action to perform. Statements are separated by semicolon (;).**

### if...else

The if statement evaluates the expression inside the parenthesis. if the result is true, it executes the block of code. If the result is false, the code inside the else block will be executed.

```js
if (condition) {
   statement1
} else {
   statement2
}
```

```js
let age = 24
if(age >= 18){
    alert("allow")
} else {
    alert("not allow")
}
```

multiple `if...else` statement

```js
if (condition1) {
   statement1
} else if(condition2) {
   statement2
} else if(condition3) {
   statement3
} else {
    statement4
}
```


### switch statement

A `switch` statement can replace multiple if checks.
The `switch` statement to select one of many code blocks to be executed.



```js
switch (x) {
  case value1:
    //Statements executed when the x === value1
    [break;]
  case value2:
    //Statements executed when the x === value2
    [break;]
  ...
  case valueN:
    //Statements executed when the x === valueN 
    [break;]
  [default:
    //Statements executed when none of the values match the value of x
    [break;]]
}
```

```js
let a = 5;

switch (a) {
  case 3:
    alert( 'Too small' );
    break;
  case 4:
    alert( 'Exactly!' );
    break;
  case 5:
    alert( 'Too big' ); // 
    break;
  default:
    alert( "I don't know such values" );
}
```

[truthy and falsy values in javascript](https://medium.com/@shindesudarshan070/truthy-and-falsy-values-in-javascript-253b705f2f72).