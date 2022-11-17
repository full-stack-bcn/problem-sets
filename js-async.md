# Asynchronous Functions

1. Rewrite the following function using `Promise`s:

   ```js
   function add(a, b) {
     return a + b;
   }
   ```

2. Rewrite the following function using `Promise`s:

   ```js
   function squareRoot(x) {
     if (x >= 0) {
       return Math.sqrt(x);
     } else {
       return { error: "'x' must be positive" };
     }
   }
   ```

3. Using the [News API](https://newsapi.org), retrieve the associated photos of
   the top headlines. Use [`axios`](https://github.com/axios/axios) to do all 
   requests:

   - First register on the News API website to get an API key (it's easy).

   - Write a script to retrieve the JSON information about the
     [top headlines](https://newsapi.org/docs/endpoints/top-headlines) for Spain.

   - Download the image of a single news article (taken form the `urlToImage`
     field) using code like this:

     ```js
     axios({
       method: "get",
       url: "https://someurl.com/some-file.jpg",
       responseType: "stream",
     }).then(function (response) {
       response.data.pipe(fs.createWriteStream("/my/dir/downloaded.jpg"));
     });
     ```

     The `fs` package is internal to NodeJS.

   - Create an array of Promises to retrieve all photos at in parallel, using
     `Promise.all`.
