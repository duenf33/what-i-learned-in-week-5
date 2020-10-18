# 😎 WHAT I LEARNED IN WEEK 5 😎

![Jim Carrey](img/typing.gif)

## 🤔 What is the difference between `map()` and `filter()`?
The `map()` method will create a new *array*, however, it will process a function given to the original *array*. It will call the provided function once for each element in the array in the same order. It does not execute the function for array elements without value and in the new output *array* will show the results. This will not change the original array at all.<br>

* Syntax ⇲<br>
```javascript
array.map(function(currentValue, index, arr), thisValue)
```
* Parameter Values<br>
  
|              **Parameter**           |                         **Description**                                                 |
|--------------------------------------|-----------------------------------------------------------------------------------------|
|  function(currentValue, index, arr)  |  Required. A function to be run for each element in the array.                          |
|                                      |         **Argument**       |       **Description**                                      |
|                                      |  currentValue              |  Required. The value of the current element                |
|                                      | index                      | Optional. The array index of the current element           |
|                                      | arr                        | Optional. The array object the current element belongs to  |
|                                                                                                                                |
|         thisValue                    |  Optional. A value to be passed to the function to be used as its "this" value. If this parameter is empty, the value "undefined" will be passed as its "this" value |

 	
Function arguments:
 	
	
 	
 	
 	

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

const newArray = numbersArray.map(myFunction)

function myFunction(num) {

  return num * 10;          // [ 430, 670, 230, 60 ]

}

console.log(newArray)
```

In the other hand...<br>
The `filter()` method is used to create a new *array* from a given *array* consisting of only those elements from the given *array* which satisfy a condition set by the argument method. 
