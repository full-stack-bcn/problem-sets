
Javascript
==========

Basic Javascript
----------------

1. Write a program that shows 100 times

   ```
   I feeel good. Na-ra na-ra na-ra na!
   ```

2. Write a program that shows the arguments that you passed:
   
   ```
   $ node show-args.js first second " third " 
   Argument[0] = "first"
   Argument[1] = "second"
   Argument[2] = " third "
   ```

3. Write a program that produces the sum of its arguments:

   ```
   $ node sum-args.js 1 2 3 4
   10
   $ node sum-args.js abra kedavra
   NaN
   ```

4. Write a program that draws a triangle like the one below given the height
   as an argument (using ``for`` and then using ``while``):

   ```
   $ node triangle.js 5
   *
   **
   ***
   ****
   *****
   ```

5. Write a program that receives 2 operands and an operation and produces the result:

   ```
   $ node expr.js 15 + 14
   29
   $ node expr.js 2 '*' 3
   6
   $ node expr.js 1234 / 16
   77.125
   ```

Arrays
------

1. Write the following functions which receive an array:
   * ``largest`` returns the largest element in the array.
   * ``trim`` returns a copy of the array without the first and last elements.
   * ``arraySum`` returns the sum of the elements.

2. Write a program that produces the sum of each column in a CSV file.
   To read the file:

   ```js
   const fs = require('fs')
   let fileContent = fs.readFileSync('some_data.csv').toString()
   ```

Objects
-------

1. Write a function ``analyzer`` that receives an object with fields ``name`` and
   ``age``:
   ```js
   console.log(analyzer({ name: 'James Bond', age: 27 }));
   ```
   and returns the following message
   ```
   Your name is James Bond and you are 27 years old.
   ```

2. Write a function ``transpose`` that receives an array of objects such as
   ```js
   [{ user: 'jlopez', password: '1234' }, 
    { user: 'pacof',  password: 'abcd' }]
   ```
   and returns an object with two fields ``users`` and ``passwords`` containing
   all the users and all the psswords collected together
   ```js
   { users: ['jlopez', 'pacof'], passwords: ['1234', 'abcd'] }
   ```

3. Convert a CSV file such as:
   ```
   name;age;weight
   james;27;85
   peter;32;56
   ```
   into a JSON file:
   ```json
   [
     { "name": "james", "age": 27, "weight": 85 },
     { "name": "peter", "age": 32, "weight": 56 }
   ]
   ```
   (In the CSV, the header indicates the names of the fields, the following lines are the objects.)

4. Write the inverse conversion as the last problem, from JSON to CSV.


Array Functional Methods
------------------------

1. Write a function ``count`` that, given an array of numbers and a callback,
   counts the number of items for which the callback returns ``true``.

2. Implement two functions, ``map`` and ``filter`` (receiving
   an array and a callback), in terms of ``forEach``.

3. Likewise, implement ``find`` in terms of ``filter`` (ignore efficiency!).

4. Implement ``some`` and ``every`` in terms of ``map`` and ``filter``.

5. Write a function ``singles`` that, given an array of numbers, returns a new
   array containing only the values of the original array that appear only once.
   Implement it in terms of ``filter``.

6. Write a function ``uniq`` that, given an array of numbers, removes
   consecutive repetitions of values. Implement it in terms of ``reduce``.

7. What do these functions do?
   ```js
   const f1 = n => [...`${n}`].map(i => parseInt(i))

   const f2 = (...nums) => nums.reduce((acc, val) => acc + val, 0) / nums.length

   const f3 = (arr, val) => arr.reduce((a, v) => (v === val ? a + 1 : a), 0)

   const f4 = (A) => A.filter((item, index) => index === arr.indexOf(item))

   const f5 = (A) => [].concat(...A)
   ```

8. Sort an array of objects such as 
   ```js
   { name: 'Fernando', lastname: 'Rodríguez', age: 39 }
   ```
   by lastname

9. Write the ``findIndex`` method as a function
   ```js
   function myFindIndex(array, fn) { /* ... */ }
   ```
