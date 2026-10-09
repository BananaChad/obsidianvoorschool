#HTML
this is used by using the `anchor` element
the anchor is a bit confusing me
its like the [[IMAGES IN HTML]] element but instead of img and alt
its a href (where the link goes) and just plain text before the closing tag
heres a quick example

```html
<a href = "https://google.com">this is google.</a>
```

<a href = "https://google.com">this is google.</a>

you can use it in combinations with paragraphs to add a clickable link IN YOUR SENTENCE

```html
<p> this is <a href = "https://google.com">google.</a></p>
```

<p> this is <a href = "https://google.com">google.</a></p>
also quick accessibility tip
use `hreflang` to tell the browser what language your link is meant to be seen in

using `target = _blank` causes the website to open in a <ins>new tab</ins> which could be useful for stuff like linking social media but not wanting them **off your website**

for stuff I didn't mention (sorry) look[here!](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

```html
<!-- you can also make clickable images! -->
<a href="https://freecatphotoapp.com"><!-- first part is the link--><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."><!--the second part is the image! --></a>
```
