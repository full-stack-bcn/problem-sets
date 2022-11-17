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

2. Download the source of the 
   [HTML 5 Test Page](https://cbracco.github.io/html5-test-page/). 
   Now add a style sheet to this page and use it to solve the following exercises:

   a. Set the font for the whole page to be "Sans-serif".

   b. Change ``h2`` headings inside ``article``s to be underlined.

   c. Distribute the links in the ``nav`` section horizontally (using *flexbox*).

   d. Put a border around ``blockquote``.

   e. Change all links to the top so that they have a border when the mouse hovers
      above them.


Page Elements
-------------

1. Put an image on the corner saying "Fork me on Github", similar to the one seen on  
   [Homebrew](https://brew.sh/).

2. Create a bottom (or top) banner for a page that says "This site uses cookies, what 
   a bummer!", and a button to "Accept all". Make it disappear when clicking the "accept" button. Investigate how to animate the banner on loading the page.

3. Create HTML and CSS to show an "alert dialog". To do it, you can add the markup
   for the dialog, position it with absolute coordinates and make it invisible at first. Add event listeners to show it when clicking a button. Also put an "ok" button in the dialog to close it.

4. Make a page in which there is a very long paragraph 
   (use [Lorem Ipsum](https://www.lipsum.com/) for some text), which only shows a small
   part, maybe 3 lines or so. Show clearly that the text is incomplete, with dots, a gradient, etc. Whenever you click the paragraph, it should expand. If you click it again, it should go back to the compressed version. Do it changing the classes of the element using the DOM.

Styling whole pages
-------------------

1. Choose a poem (or short text) that you like and make a page for it. Choose 
   appropriate fonts and styles for its content.

2. Style the bookmarks you made in the HTML exercises. Make links as square icons
   with styles for hover to detect mouse presence. Put icons to the links to make
   them easy to recognize.

3. Download the HTML file from [CSS Zen Garden](http://csszengarden.com) and
   style it. (Do not take inspiration from existing designs.)

4. Work on a style for the whole 
   [HTML 5 TestPage](https://cbracco.github.io/html5-test-page/).

