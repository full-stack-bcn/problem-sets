# Javascript: Array Functional Methods

1. Determine what these functions do and give them a good name:

   ```js
   const f1 = (n) => [...`${n}`].map((i) => parseInt(i));
   const f2 = (...nums) => nums.reduce((acc, val) => acc + val, 0) / nums.length;
   const f3 = (arr, val) => arr.reduce((a, v) => (v === val ? a + 1 : a), 0);
   const f4 = (A) => A.filter((item, index) => index === arr.indexOf(item));
   const f5 = (A) => [].concat(...A);
   ```

2. Write a function `count` that, given an array of numbers and a callback,
   counts the number of items for which the callback returns `true`.

3. Implement two functions, `map` and `filter` (receiving
   an array and a callback), in terms of `forEach`.

4. Likewise, implement `find` in terms of `filter` (ignore efficiency!).

5. Implement `some` and `every` in terms of `map` and `filter`.

6. Write a function `singles` that, given an array of numbers, returns a new
   array containing only the values of the original array that appear only once.
   Implement it in terms of `filter`.

7. Write a function `uniq` that, given an array of numbers, removes
   consecutive repetitions of values.

8. Implement the `uniq` function of the last exercise in terms of `reduce`.

9. Sort an array of objects such as

   ```js
   {
     name: 'Fernando',
     lastname: 'Rodríguez',
     age: 39
   }
   ```

   by lastname

10. Write the `findIndex` method as a function

    ```js
    function myFindIndex(array, fn) {
      /* ... */
    }
    ```

11. Write a function `rotateArray(array, n)` which rotates an array by n
    positions. For example: `rotateArray([1, 2, 3, 4, 5], 2)` will return
    `[4, 5, 1, 2, 3]`.
