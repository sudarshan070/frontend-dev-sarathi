## String Methods

In JavaScript, the textual data is stored as strings. There is no separate type for a single character.

### String.charAt()

charAt() is a method that returns the character from the specified index.

```js
charAt(index)

let str = "Sarathi frontend development"

console.log(str.charAt(4)) // t
console.log(str.charAt(9)) // r
```

### String.charCodeAt()

The charCodeAt() method returns an integer between 0 and 65535 representing the UTF-16 code unit at the given index.

```js
charCodeAt(index)

let str = "Sarathi frontend development"
console.log(str.charCodeAt(4)) // 116
console.log(str.charCodeAt(9)) // 114 (char code of t is 116 and r is 114)
```

### String.concat()

The concat() method concatenates the string arguments to the calling string and returns a new string.

```js
let str1 = "Frontend"
let str2 = "Developer"

console.log(str1.concat(" ", str2)) // Frontend Developer
```

### String.includes()

The includes() method performs a case-sensitive search to determine whether one string may be found within another string, returning true or false as appropriate.

```js
let str = "Sarathi frontend development"

console.log(str.includes("Sarathi")) // true
console.log(str.includes("d")) // true
console.log(str.includes("D")) // false
```

### String.indexOf()

The indexOf() method returns the index within the calling String object of the first occurrence of the specified value, starting the search at fromIndex. Returns -1 if the value is not found.

```js
let str = "Sarathi frontend development"

console.log(str.indexOf("d")) // 15
```

### String.repeat()

The repeat() method constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together.

```js
let str = "Sarathi frontend development"

console.log(str.repeat(3)) // Sarathi frontend developmentSarathi frontend developmentSarathi frontend development
```

### String.replace()

The JavaScript String replace() method returns a new string with a substring (substr) replaced by a new one (newSubstr). The repalce() method doesn't change original string.

```js
let newStr = str.replace(substr, newSubstr);

let str = "Sarathi frontend development"

let newStr1 = str.replace("frontend", "front-end")

console.log(newStr1) // Sarathi front-end development
```

### String.Slice()

The slice() method extracts a section of a string and returns it as a new string, without modifying the original string.

```js
let str = "Sarathi frontend development"

console.log(str.slice(4)) // frontend development
console.log(str.slice(0, 12)) // Sarathi fron
```

### String.split()

The split() method divides a String into an ordered list of substrings, puts these substrings into an array, and returns the array. 

```js
let str = "Sarathi frontend development"

console.log(str.split()) // ["Sarathi frontend development"]
console.log(str.split(" ")) // ["Sarathi", "frontend", "development"]
```


### String.substring()

The substring() method returns the part of the string between the start and end indexes, or to the end of the string.

```js
let str = "Sarathi frontend development"

console.log(str.substring(8)) // frontend development
console.log(str.substring(0, 16)) // Sarathi frontend
```

### String.toLocalLowerCase()

The toLocaleLowerCase() method returns the calling string value converted to lower case

```js
let str = "Sarathi Frontend Development"

console.log(str.toLocalLowerCase()) // "sarathi frontend development"
```

### String.toLocalUpperCase()

The toLocaleUpperCase() method returns the calling string value converted to Upper case

```js
let str = "Sarathi frontend development"

console.log(str.toLocalUpperCase()) // "SARATHI FRONTEND DEVELOPMENT"
```


### String.trim()

The trim() method removes whitespace from both ends of a string.

```js
let str = "    Sarathi frontend development     "

console.log(str.trim()) // "Sarathi frontend development"
```