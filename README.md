# 😎 **WHAT I LEARNED IN WEEK 5** 😎

![Jim Carrey](img/typing.gif)

## 🤔 **What is the difference between `map()` and `filter()`?** 🤔
**The `map()` method** will create a new *array*, however, it will process a function given to the original *array*. It will call the provided function once for each element in the array in the same order. It does not execute the function for array elements without value and in the new output *array* will show the results. This will not change the original array at all.<br>

* Syntax ⇲<br>
```javascript
array.map(function(currentValue, index, arr), thisValue);
```
* Parameter Values ⇲<br>

|              **Parameter**           |     **Description**        |                                                            |
| ------------------------------------ | -------------------------- | ---------------------------------------------------------- |
|  function(currentValue, index, arr)  |  Required. A function to be run for each element in the array.                          |
|                                      |         **Argument**       |       **Description**                                      |
|                                      |  currentValue              |  Required. The value of the current element                |
|                                      | index                      | Optional. The array index of the current element           |
|                                      | arr                        | Optional. The array object the current element belongs to  |
|         thisValue                    |  Optional. A value to be passed to the function to be used as its "this" value. If this parameter is empty, the value "undefined" will be passed as its "this" value |

* Examples ⇲<br>
```javascript
const ages = [25, 36, 49, 64, 81];

const example = function() {

const output = ages.map(Math.sqrt);

return output;

};

console.log(example());     // [ 5, 6, 7, 8, 9 ]
```

```javascript
const numbersArray = [43, 67, 23, 6];

const newArray = numbersArray.map(myFunction);

function myFunction(num) {

  return num * 10;          // [ 430, 670, 230, 60 ]

}

console.log(newArray);
```

In the other hand...<br>
**The `filter()` method** is used to create a new *array* from a given *array* consisting of only those elements from the given *array* which satisfy a condition set by the argument method.<br>

* Syntax ⇲<br>
```javascript
array.filter(function(currentValue, index, arr), thisValue)
```
* Parameter Values ⇲<br>

|              **Parameter**           |     **Description**        |                                                            |
| ------------------------------------ | -------------------------- | ---------------------------------------------------------- |
|  function(currentValue, index, arr)  |  Required. A function to be run for each element in the array.                          |
|                                      |         **Argument**       |       **Description**                                      |
|                                      |  currentValue              |  Required. The value of the current element                |
|                                      | index                      | Optional. The array index of the current element           |
|                                      | arr                        | Optional. The array object the current element belongs to  |
|         thisValue                    |  Optional. A value to be passed to the function to be used as its "this" value. If this parameter is empty, the value "undefined" will be passed as its "this" value |

* Here below we have an example ⇲<br>
```javascript
function greaterThan(num) {

  return num >= 10;

}

let filterArr = [12, 5, 8, 130, 44].filter(greaterThan);      // filterArr is [12, 130, 44]
```
---

## ♻️ **The `For-Of` Loop** ♻️<br>
The JavaScript `For-Of` statement, loops through the values of an iterable objects.<br>

For-Of lets you loop over data structures that are iterable such as *Arrays*, *Strings*, *Maps*, and more.<br>

* Syntax ⇲
```javascript
for (variable of iterable) {

  // code block to be executed

};
```
* Here below we have some examples on how it is implemented ⇲
```javascript
const arr = ['a', 'b'];

for (const letter of arr) {

    console.log(letter);

};
// Output:
// a
// b
```
---
## 📦 **`Objects`**
`Objects` can be created with brackets `{...}`, are able to store a variety of data of any kind. `Objects` are the main core of programming and pretty much everything. Its very important to learn as much as we can from them to become better programmers.<br>

An `object` can be created as empty with one or two syntaxes such as... ⇲<br> 
```javascript
let user = new Object(); // "object constructor" syntax

let user = {};  // "object literal" syntax
```

...as where we would be able to store any lists of properties in the future as a `key: value` pair. Where `key` also known as`property name` is a string and `value` could be anything.<br>

In JavaScript everything, except primitive values, are objects ⇲<br>

>* **`Booleans`**  can be objects (if defined with the new keyword)<br>
>* **`Numbers`** can be objects (if defined with the new keyword)<br>
>* **`Strings`** can be objects (if defined with the new keyword)<br>
>* **`Dates`** are always objects<br>
>* **`Maths`** are always objects<br> 
>* **`Regular expressions`** are always objects<br>
>* **`Arrays`** are always objects<br>
>* **`Functions`** are always objects<br>
>* **`Objects`** are always objects<br>

JavaScript defines 5 types of primitive data types ⇲

>* `string`
>* `number`
>* `boolean`
>* `null`
>* `undefined`

A primitive value is a value that has no properties or methods.
Primitive values are immutable