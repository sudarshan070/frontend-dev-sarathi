## Array Methods

In JavaScript, arrays can be a collection of elements of any type. This means that you can create an array with elements of type String, Boolean, Number, Objects, and even other Arrays. 

```js
let array = [1, 'a', 'sarathi' {a: "one", b: "two"}, [1,2,3]]
```

There are two syntaxes for creating an empty array.
```js
let arr = new Array()
 arr = []
```

Array elements are numbered(index), starting with zero.
We can get an element by its number(index) in square brackets.
```js
let arr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

console.log(arr[0]) // "Aniket"
console.log(arr[1]) // "Krushna"
console.log(arr[2]) // "Mayank"
console.log(arr[5]) // "Virat"
```


### Array.push

The push() method adds one or more elements to the end of an array and returns the new length of the array.

```js
let arr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit"]
arr.push("Virat")
console.log(arr) // ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
```

### Array.pop()

The pop() method removes the last element from an array and returns that element. This method changes the length of the array.

```js
let arr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit"]
console.log(arr.pop()) // "Rohit"
console.log(arr) // ["Aniket", "Krushna", "Mayank", "Sachin"]

```

### Array.shift()

The shift() method removes the first element from an array and returns that removed element. This method changes the length of the array.

```js
let arr  = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
arr.shift()
console.log(arr) // ["Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
```


### Array.unshift()

The unshift() method adds one or more elements to the beginning of an array and returns the new length of the array.

```js
let arr = ["Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
arr.unshift("Aniket")
console.log(arr) // ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
```

### Array.from

The Array.from() static method creates a new, shallow-copied Array instance from an array-like or iterable object.

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

The every() method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.

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

The find() method returns the value of the first element in the provided array that satisfies the provided testing function. If no values satisfy the testing function, undefined is returned.

```js
let arr = [89,12, 34, 74, 87, 90]

console.log(arr.find(ele => ele < 90 )) // 89
```

### Array.findIndex()

The findIndex() method returns the index of the first element in the array that satisfies the provided testing function. Otherwise, it returns -1, indicating that no element passed the test.

```js
let arr = [89,12, 34, 74, 87, 90]

console.log(arr.findIndex(ele => ele < 90 )) // 0

let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

newArr.findIndex(ele => ele == "Virat") // 5
```

### Array.flat()

The flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.

```js
let arr = [89,12, 34, 74, 87, 90,[1,2,3]]
console.log(arr.flat()) // [89, 12, 34, 74, 87, 90, 1, 2, 3]
```

### Array.includes()

The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

newArr.includes("Aniket") //true

```

### Array.indexOf()

The indexOf() method returns the first index at which a given element can be found in the array, or -1 if it is not present.

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

The reverse() method reverses an array. The first array element becomes the last, and the last array element becomes the first.
```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

console.log(newArr.reverse()) // ["Virat", "Rohit", "Sachin", "Mayank", "Krushna", "Aniket"]
```

### Array.slice()

The slice() method returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end represent the index of items in that array.

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

console.log(newArr.slice(1,4)) //  ["Krushna", "Mayank", "Sachin"]
```


### Array.some()

The some() method tests whether at least one element in the array passes the test implemented by the provided function. It returns true if, in the array, it finds an element for which the provided function returns true; otherwise it returns false.

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
console.log(newArr.some(ele => ele == "aniket")) // false
console.log(newArr.some(ele => ele == "Aniket")) // true


let arr1 = [1, 2, 3, 4]
console.log(arr1.some(e => e % 2 == 0)) //true
```

### Array.sort()

The sort() method sorts the elements of an array and returns the sorted array.

```js
let arr = [1,4,3,2,5,7,6,9,0,8]
 console.log(arr.sort()) // [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

 console.log(arr.sort((a,b) => b - a)) // [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```
### Array.splice()

The splice() method changes the contents of an array by removing or replacing existing elements and/or adding new elements.

```js
let newArr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
newArr.splice(1,0,"Rahul")
console.log(newArr) //  ["Aniket", "Rahul", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]

let num = [0, 1, 2, 3, 4, 5]
num.splice(6,0,6)
console.log(num) //  [0, 1, 2, 3, 4, 5, 6]
```

### Array.filter()

The filter() method creates a new array with all elements that pass the test implemented by the provided function. It will return same size of array or smaller than.

```js
let arr = ["Aniket", "Krushna", "Mayank", "Sachin", "Rohit", "Virat"]
let filterArr =  arr.filter(e => e.length > 5)
console.log(filterArr) // ["Aniket", "Krushna", "Mayank", "Sachin"]


let num = [0, 1, 2, 3, 4, 5]
let filterNum = num.filter(e => e % 2 == 0)
console.log(filterNum) // [0, 2, 4]
```

### Array.forEach()

The forEach() method executes a provided function once for each array element. forEach return undefined.

```js
let arr = ["Aniket", "Krushna", "Mayank"]
arr.forEach(e => console.log(e))
// Aniket
// krushna
// Mayank
```


### Array.map()

The map() method creates a new array populated with the results of calling a provided function on every element in the calling array. Return same size of array.

```js
let arr = [ 1, 2, 3, 4, 5]
let mapArr = arr.map(num => num * 2) 
console.log(mapArr) // [2, 4, 6, 8, 10]
```

### Array.reduce()

The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.

```js
let arr = [ 1, 2, 3, 4, 5]
let reduceArr = arr.reduce((acc ,cv) => acc + cv, 0)
console.log(reduceArr) // 15
```
