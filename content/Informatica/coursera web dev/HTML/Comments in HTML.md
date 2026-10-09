comments are well, comments. For any comments or todos that you want to change in your code you add a _comment_. Example

i want a paragraph to be changed to a sentence, but i cant change this at the moment, i put a comment to remind me to remove it

```html
<html>
  <body>
    <!--
    TODO: delete this paragraph as its no longer needed.
    -->
    <p>test paragraph<p>
  </body>
</html>
```

comments always start with < !-- and end with --> (remove the space at the !)
if you forget to put down a comment errors will pop up and your code will break, as your program will think your comment is part of the code

```html
<html>
  <body>
    -->
    TODO: delete this paragraph as its no longer needed.
    <!--
    <p>test paragraph<p>
  </body>
</html>
```

if you do the order wrong, you will accidentally comment the code **under** your comment, which causes the code to not to run

```html
<html>
  <body>
    TODO: delete this paragraph as its no longer needed.
    <p>test paragraph<p>
  </body>
</html>
```

if you dont add the comment characters at all, your code will throw errors as it doesnt know what it means.

# Ways to Use Comments

a commonly used way to use comments is to explain what code is doing and write any additional code that you want to add in the future. Quick examples below:

explaining what the code does:

```html
<html>
  <body>
   <!-- this paragraph is used to explain what our company does -->
    <p>we as a company build train infrastructure so you can ride safely on your trains.<p>
  </body>
</html>
```

asking other developers to do something for you (like CSS developers!)

```html
<html>
  <body>
	<!-- please make all buttons orange, including this one! -->
	<button>Click me</button>
  </body>
</html>
```
