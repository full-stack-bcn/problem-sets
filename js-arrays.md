# Arrays

1. Write a function `largest` which returns the largest element in an array
   of numbers.

2. Write a function `trim` which returns a copy of an array removing the
   elements at the beginning or end that are `null`.

3. Write a function `arraySum` which returns the sum of the elements in an array.

4. Write a program that produces the sum of each column in a CSV file.
   To read the file:

   ```js
   const fs = require("fs");
   let fileContent = fs.readFileSync("some_data.csv").toString();
   ```

5. Write a function `countAppearances` which receives an array of strings `A`
   (a list of words) and a string `w` (a single word), and returns how many
   times `w` appears in `A`.

6. Write a function `reverse` which receives an array and returns a new array
   with the same elements in reverse order. If the input array is
   `[1, 2, 3, 4, 5]`, the function should return `[5, 4, 3, 2, 1]`.

7. Write a function `aboveAverage` that receives an array of numbers and
   returns the fraction (between 0.0 and 1.0) of numbers in the array the are
   greater than the average of the array.

8. Write a function `firstNonRepeated` that receives a string like
   `"aabbcdddeffgh"` and returns the first letter in the string which doesn't
   have consecutive repetitions (in the example would be `e`).

9. In the game of Fizz Buzz, kids take turns in saying the natural numbers, but
   when a number is divisible by 3, they say "Fizz", when the number is
   divisible by 5 they say "Buzz", and when the number is divisible by 3 and 5
   they say "Fizz Buzz". If you put the consecutive responses (either an
   integer or a string) in an array it would look like:

   ```js
   [
     1,
     2,
     "Fizz",
     4,
     "Buzz",
     "Fizz",
     7,
     8,
     "Fizz",
     "Buzz",
     11,
     "Fizz",
     13,
     14,
     "FizzBuzz" /* ... */,
   ];
   ```

   Write a function that receives an integer length N as a parameter and
   produces the `FizzBuzz` array of length N.

10. Write a function `range(a, b)` that receives two integers and produces an
    array with the consecutive numbers starting at `a` but excluding `b`. For
    instance, `range(4, 10)` produces `[4, 5, 6, 7, 8, 9]`.

11. Write a function that receives an array of arrays of numbers, such as
    `[[1, 2, 3], [100, 10], [-5, -7]]` and returns an array with the minimum
    values in each array, that is: `[1, 10, -7]`.

12. Write a function `duplicate` which receives an array and an integer `n` and
    returns a new array with `n` concatenated copies of the original array.

13. Write a function that receives two arrays `A` and `B` and returns an
    array with the elements in `A` that are not present in `B`.

14. Write a function that receives two strings and returns `true` if they are
    [anagrams](https://en.wikipedia.org/wiki/Anagram). Two Spanish words that
    are anagrams are "esponja" and "japones" (accents/tildes are not taken into
    account).

15. Write a function that receives a string and reverses the order of all the
    vowels in the string: `reverseVowels("I love burritos")` gives
    `"o livu berrotIs`.

16. Given an array of integers (let's call it `x`), calculate the percentage
    for the number of positive integers, negative integers, and zeros in `x`.

17. Write a function that receives an array of numbers, and returns the
    [median](https://en.wikipedia.org/wiki/Median).
