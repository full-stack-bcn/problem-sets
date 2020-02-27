
Javascript
==========

Basic Javascript
----------------

1. Write a Javascript script/program that shows 100 times on the console:

   ```
   I feeel good. Na-ra na-ra na-ra na!
   ```

1. Write a Javascript script in an HTML document that produces 100 paragraphs
   with the text "I really know how to generate some DOM, you know?". To create
   a paragraph and add it to the ``<body>`` use code analogous to:
   ```js
   let p = document.createElement('p');
   p.innerText = "a new paragraph";
   document.body.appendChild(p);
   ```

1. Write a NodeJS program that shows the arguments that you passed:
   
   ```
   $ node show-args.js first second " third " 
   Argument[0] = "first"
   Argument[1] = "second"
   Argument[2] = " third "
   ```

1. Write a NodeJS program that produces the sum of its arguments:

   ```
   $ node sum-args.js 1 2 3 4
   10
   $ node sum-args.js abra kedavra
   NaN
   ```

1. Write a program that draws a triangle like the one below given the height
   as an argument (using ``for`` and then using ``while``):

   ```
   $ node triangle.js 5
   *
   **
   ***
   ****
   *****
   ```

1. By using ``document.createElement`` and ``document.body.appendChild``, create
   an HTML page which at loading time adds 100 paragraphs to the ``<body>`` each
   one with the text "This is paragraph N", N being its index.

1. Write a program that receives 2 operands and an operation and produces the result:

   ```
   $ node expr.js 15 + 14
   29
   $ node expr.js 2 '*' 3
   6
   $ node expr.js 1234 / 16
   77.125
   ```

1. Write an HTML document that is a calculator (with all buttons and operations,
   etc). Implement the basic arithmetic operations, like in a calculator, as
   well as the "C" key (which erases pending operations and clear the number).

1. Write a document with many elements in the body and remove the first 5 from
   it using a script. (The ``remove`` method removes it from the DOM.)


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

3. Write a function ``appearances`` which receives an array of strings ``A`` (a
   list of words) and a string ``w`` (a word), and returns how many times ``w``
   appears in ``A``.

4. Write a function ``reverse`` which receives an array and returns a new array
   with the same elements in reverse order. If the input array is ``[1, 2, 3, 4, 5]``, 
   the function should return ``[5, 4, 3, 2, 1]``.

5. Write a function ``aboveAverage`` that receives an array of numbers and
   returns the fraction (between 0.0 and 1.0) of numbers in the array the are
   greater than the average of the array.

6. Write a function ``firstNonRepeated`` that receives a string like
   ``"aabbcdddeffgh"`` and returns the first letter in the string which doesn't
   have consecutive repetitions. 

7. In the game of Fizz Buzz, kids take turns in saying the natural numbers, but
   when a number is divisible by 3, they say "Fizz", when the number is
   divisible by 5 they say "Buzz", and when the number is divisible by 3 and 5
   they say "Fizz Buzz". If you put the consecutive responses (either an integer
   or a string) in an array it would look like:
   ```js
   [1, 2, "Fizz", 4, "Buzz", "Fizz", 7, 8, "Fizz", "Buzz", 11, "Fizz", 13, 14, "FizzBuzz", ...]
   ```
   Write a function that receives an integer length N as a parameter and
   produces the "FizzBuzz" array of length N.

8. Write a function ``range(a, b)`` that receives two integers and produces an
   array with the consecutive numbers starting at ``a`` but excluding ``b``. For
   instance, ``range(4, 10)`` produces ``[4, 5, 6, 7, 8, 9]``.

9. Write a function that receives an array of arrays of numbers, such as 
   ``[[1, 2, 3], [100, 10], [-5, -7]]`` and returns an array with the minimum 
   values in each array, that is: ``[1, 10, -7]``.

10. Write a function that receives two arrays ``A`` and ``B`` and returns an
    array with the elements in ``A`` that are not present in ``B``.

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

DOM
---

1. Generate the following HTML element programmatically in Javascript and add it
   to the ``<body>`` of the page
   ```html
   <div class="user">
      <img href="/png/bond.png">
      <span class="name">James Bond</span>
   </div>
   ```
   Check with the Browser inspector that the structure is correct.


Mini-projects
-------------

1. Write a function that receives an integer N and returns the spelling of N
   in English (or Spanish, or Catalan). Examples
   ```
   say(19) => "nineteen"
   say(42) => "Forty-two"
   say(100) => "One hundred"
   say(467889) => "Four hundred sixty-seven thousand eight hundred eighty-nine"
   ```
