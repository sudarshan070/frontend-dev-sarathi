## Scheduling: setTimeout and setInterval

### setTimeout()

setTimeout() runs the code/function once of the timeout

```js
setTimeout(expression, timeout, arg, arg1, ...)

setTimeout(alert("Frontend Developer"), 1000)

setTimeout(() => alert("Frontend Developer"), 1000)

setTimeout(function(){
    alert("Frontend Developer")
}, 1000)

function dev(){
alert("Frontend Developer")
}
setTimeout(dev, 1000)

function jsDev(name){
    console.log(`${name} is JavaScript Developer`)
}
setTimeout(jsDev, 1000, "Aniket")
```

### clearTimeout()

The clearTimeout() function in javascript clears the timeout which has been set by setTimeout()function before that.

```js
let timeoutId = setTimeout(...);
clearTimeout(timeoutId);

let timeoutId = setTimeout(() => console.log("never happens"), 1000);
console.log(timeoutId); 
clearTimeout(timeoutId);
```


### setInterval()

setInterval() runs the code/function repeatedly, with the length of the timeout between each repeat.

```js
setTimeout(expression, timeout, arg, arg1, ...)

setTimeout(alert, 1000); // Will alert once, after a second.

let intervalID = setInterval(myCallback, 1000, 'Frontend', 'developer');
function myCallback(para1, para2 ){
 console.log(para1, para2); 
}

```

### clearInterval()

The clearInterval() function in javascript clears the interval which has been set by setInterval() function before that. It is return value undefined.

```js
let intervalId = setTimeout(alert, 1000);

clearInterval(intervalID)
```