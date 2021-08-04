## Array Methods

### Array.from

```js
let str = "Aniket"

console.log(Array.from(str)) //["A", "n", "i", "k", "e", "t"]

```


### Array.concat

The concat() method is used to merge two or more array. It does not change existing array.

```js
let arr1 = [1, 2, 3, 4]
let arr2 = [5, 6, 7,8]

let arr = arr1.concat(arr2)
console.log(arr) // [1, 2, 3, 4, 5, 6, 7, 8]
```


### Array.every() 

```js
let arr2 = [5, 6, 7,8]

let isSmall = (cv) => cv < 8

arr2.every(isSmall) // false
```

### Array.fill()

The fill() method changes the all elements in an array. It return modified array.

```js
let arr2 = [5, 6, 7,8]
let arr = arr2.fill(5, 2)

console.log(arr)  // [5, 6, 5, 5] 
```


### Array.find()

```js
let arr = [89,12, 34, 74, 87, 90]

console.log(arr.find(ele => ele < 90 )) // 89
```

### Array.findIndex()

```js
let arr = [89,12, 34, 74, 87, 90]

console.log(arr.findIndex(ele => ele < 90 )) // 0

let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

newArr.findIndex(ele => ele == "Virat") // 5
```

### Array.flat()

```js
let arr = [89,12, 34, 74, 87, 90,[1,2,3]]
console.log(arr.flat()) // [89, 12, 34, 74, 87, 90, 1, 2, 3]
```

### Array.includes()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

newArr.includes("Aniket") //true

```

### Array.indexOf()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat", "Mayank"]
newArr.indexOf("Mayank") // 2

newArr.indexOf("Mayank", 4) // 6
```

### Array.join()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat", "Mayank"]
console.log(newArr.join()) // "Aniket,Krushna,Mayank,Sachin,Rohit,Virat,Mayank"
```

### Array.reverse()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

console.log(newArr.reverse()) // ["Virat", "Rohit", "Sachin", "Mayank", "Krushna", "Aniket"]
```

### Array.slice()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

console.log(newArr.slice(1,4)) //  ["Krushna", "Mayank", "Sachin"]
```


### Array.some()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
console.log(newArr.some(ele => ele == "aniket")) // false
console.log(newArr.some(ele => ele == "Aniket")) // true


let arr1 = [1, 2, 3, 4]
console.log(arr1.some(e => e % 2 == 0)) //true
```


### Array.splice()

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
newArr.splice(1,0,"Rahul")
console.log(newArr) //  ["Aniket", "Rahul", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

let num = [0, 1, 2, 3, 4, 5]
num.splice(6,0,6)
console.log(num) //  [0, 1, 2, 3, 4, 5, 6]
```