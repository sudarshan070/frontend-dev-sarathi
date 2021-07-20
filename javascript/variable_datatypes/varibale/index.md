## Variables

**A variable is a *“named storage”* for data. We can use variables to store goodies, visitors, and other data.**

```js
 let userName;
 userName = "Rohit" // store the string
 let num = 12 // store number
``` 

JavaScript uses three keyword to declare variable.

1. var
2. let 
3. const

One of the features that came with ES6 is the addition of `let` and `const`. `var` in older script.

### variable naming

* The name must contain only letters, digits, or the symbols `$` and `_`.
* The first character must not be a digit.
* When the name contains multiple words, camelCase is commonly used. e.g. `userName`.

### var

 * Before the advent of ES6, `var` declarations ruled.
 * Variables declared using `var`, they can be re-declared or reassigned.
 ```js
 var user = "Rahul"
 var user = "Rhoit"

 var firstName = "Rahul"
 firstName = "Bantu"
 ```
 * `var` is function scoped when it is declared within a function and `var` is global scoped when it is declared outside a function.

 ```js 
if(true){
  var name = "hello"
}
console.log(name) // "hello"

function newFunction() {
    var hello = "hello";
} 
console.log(hello); // error hello is not defined
  ```
 

### let 

 * `let` is now preferred for variable declaration.
 * Variables declared using `let` they can be reassigned.
 ```js
  let lastName = "Sharma"
  lastName = "Bhat"

  let mySelf = "Raghu"
  let mySelf = "Ganesh" // error: Identifier 'mySelf' has already been declared
  ```
  * `let` is block scoped

```js
 function letTest() {
  let x = 1;
  {
    let x = 2;  // different variable
    console.log(x);  // 2
  }
  console.log(x);  // 1
 }
```

### const

 * Variables declared using `const` are called “constants”. They cannot be reassigned.
  ```js 
   let myBirthdate = 15.05.2000;
    myBirthdate = 16.05.2000; // error: Assignment to constant variable
  ```  
 * `const` declared block scope