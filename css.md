CSS
===

Basic CSS
---------

1. Make an HTML page with 3 square boxes of different colors.

2. Make an HTML page with a top menu with a logo at the left and some sections
   like "home", "services", "blog", etc. Add a fake search bar on the right. Add
   a footer at the bottom with information like the Copyright, "about",
   "contact", etc.

3. Make an HTML page which looks like a chess board. (It is forbidden to use ``table``s!)

4. Write a page with a very big text exactly centered in the middle of the page.
   Resize the browser and check that it stays perfectly centered.



Styling snippets
----------------

1. Copy this page to a file called ``login-form.html`` and style it so that the
   input boxes are aligned
   ```html
   <!doctype html>
   <html>
     <head><title>Login</title></head>
     <body>
       <form method="get" action="/user">
         <p><label>User <input type="text"></label></p>
         <p><label>Password <input type="password"></label></p>
       </form>    
     </body>
   </html>
   ```

The following series of exercises require you to first download the source of
the [HTML 5 Test Page](https://cbracco.github.io/html5-test-page/). Now add a
style sheet to this page and use it to solve the following exercises:

2. Set the font for the whole page to be "Sans-serif".

3. Change ``h2`` headings inside ``article``s to be underlined.

4. Distribute the links in the ``nav`` section horizontally (using *flexbox*).

5. Put a border around ``blockquote``.

6. Change all links to the top so that they have a border when the mouse hovers
   above them.



Styling whole pages
-------------------

1. Download the HTML file from [CSS Zen Garden](http://csszengarden.com) and
   style it. (Do not take inspiration from existing designs.)

2. Work on a style for the whole 
   [HTML 5 TestPage](https://cbracco.github.io/html5-test-page/).