## Loop Statements

 **What is loop?**
  Loop is a sequence of instructions that is continually repeated until a certain condition is reached.

   ### for loop

   A "for" loop repeats until a specified condition evaluates to false.

   ```js
   for(begin; condition; step){
       // statement
   }
   ```
  ```js
  for(let i = 0; i < 4; i++){
      console.log(i) // 0, 1, 2, 3
  }
  ```


  ### while loop

  A "while" statement executes its statements as long as a specified condition evaluates to true. 

 ```js
 while(condition){
     // statement
 }
 ```
 ```js
 let i = 0
 while(i < 3){
     console.log(i) // 0, 1, 2
     i++
 }

 let n = 0
 while(n < 3){
     i++
 }
 console.log(n)
 ```


 ### do...while loop

 The do...while statement repeats until a specified condition evaluates to false.

```js
do{
    //statement
} while(condition)
```

```js
let i = 0;
do {
  console.log( i ); // 0, 1, 2
  i++;
} while (i < 3);
```

### for...in

The "for...in" statement iterates a specified variable over all the enumerable properties of an object.

```js
for(variable in object){
    // statement
}
```

```js
let obj = {
    a:1,
    b:2,
    c:3
}

for(let i in obj){
    console.log(`${i} = ${obj[i]}`) // a = 1, b = 2, c = 3
}
```


### for...of

The "for...of" statement creates a loop iterating over iterable objects.

```js
for (variable of iterable) {
  statement
}
```

```js
let iterable = [10, 20, 30];

for (let value of iterable) {
  console.log(value); // 10, 20, 30
}
```