# Objects

1. Write a function `analyzer` that receives an object with fields `name` and
   `age`:

   ```js
   analyzer({ name: "James Bond", age: 27 });
   ```

   and shows the following message on the console:

   ```
   Your name is James Bond and you are 27 years old.
   ```

2. Write a function `transpose` that receives an array of objects such as

   ```js
   [
     { user: "jlopez", password: "1234" },
     { user: "pacof", password: "abcd" },
   ];
   ```

   and returns an object with two fields `users` and `passwords` containing
   all the users and all the passwords collected together preserving the order:

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

   (In the CSV, the header indicates the names of the fields, the following
   lines are the objects.)

4. Write the inverse conversion as the last problem, from JSON to CSV.

5. Write a function that, given an array of "fields" like:

   ```js
   [
     { field: "name", value: "James Bond" },
     { field: "age", value: 27 },
     { field: "agentNum", value: "007" },
   ];
   ```

   returns and object with those fields and values. In the example, the
   returned object should be:

   ```js
   { name: 'James Bond', age: 27, agentNum: '007' }
   ```

6. Write a function `fieldNames` that returns an array with the names of all  
   the fields in an object given as the first parameter.
