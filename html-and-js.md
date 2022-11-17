# HTML and Javascript

1. Go to a webpage, identify an element in the DOM (an ad or something annoying
   like a cookie form) and erase it from the Javascript console using `document.querySelector` or `document.getElementById`.

2. Write a Javascript script in an HTML document that produces 100 paragraphs
   with the text "I really know how to generate some DOM, you know?".

   To create a paragraph and add it to the `<body>` use code like:

   ```js
   let p = document.createElement("p");
   p.innerText = "a new paragraph";
   document.body.appendChild(p);
   ```

3. Generate the following HTML element programmatically in Javascript and add it
   to the `<body>` of the page (don't user `innerHTML` at all!):

   ```html
   <div class="user">
     <img href="/png/bond.png" />
     <span class="name">James Bond</span>
   </div>
   ```

   Check with the Browser inspector that the structure is correct.

4. By using `document.createElement` and `document.body.appendChild`, create
   an HTML page which at loading time adds 50 paragraphs to the `<body>` each
   one with the text `This is paragraph N`, N being its index.

5. Write a page that has a text input and a button and when you press the button
   computes a simple operation, which consists of two numbers with an operator
   in between and shows it on the page. For example, if you input `5 + 3`, it
   shows `8`, and with `20 * 21` it shows `4020`.

6. Write an HTML document that is a calculator (with all buttons and operations,
   etc). Implement the basic arithmetic operations, like in a calculator, as
   well as the "C" key (which erases pending operations and clear the number).

7. Write a document with many elements in the body and make them disappear
   (`remove` them from their parent) when they are clicked.
