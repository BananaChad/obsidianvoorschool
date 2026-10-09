HTML attributes are special words used inside the opening tag of an element to control the element's behavior. The `src` attribute in an `img` element specifies the image's URL (where the image is located).

Here is an example of an `img` element with a `src` attribute pointing to the freeCodeCamp logo:

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
```
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
yup cute cat ngl

# Alternate Text
All `img` elements should have an `alt` attribute. The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load. For example, `<img src="cat.jpg" alt="A cat">` has an `alt` attribute with the text `A cat`.

to add a description to your image check out
# The Figure Element!

```html
<figure>
	<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
	<figcaption>Cats love lasagna.</figcaption>     
</figure>
```
what a figure does is make it so that the image in the figure can be customized(?)

in the example above you can add **closer** text to the image then you would with a[[what are headers|header!]] 
quick example below:
![[Pasted image 20231031115224.webp]]
the first line of text is a `figcaption`
the second line of text is a `header`
see what i mean?