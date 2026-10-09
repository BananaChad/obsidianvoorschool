#HTML
sectioning off your code to prevent it from being tampered with by other elements is done like so:

```html
<h1>hello</h1>
<section>
	<h2>hi</h2>
</section>
```

i dont know what this does _yet_ but it is useful for making your code more managed than just having garbled elements everywhere

# Lists

lists are well

- bullet points!

you make them like so

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

ul stands for unordered list. they dont have an order so there doesnt have to be an indicator of letters

unordered list  |  ordered list
\----        |          ----
\- food | 1. food
\- water | 2. water

there's some neat tricks you can do mentioned [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul#ordered_list_inside_unordered_list">)

some are:

# <ins>ordered List inside Unordered list</ins>

```html
<ul>
  <li>first item</li>
  <li>
    second item
    <!-- Look, the closing </li> tag is not placed here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
    <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>
```

<ul>
  <li>first item</li>
  <li>
    second item
    <!-- Look, the closing </li> tag is not placed here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
    <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>
pretty neat huh?
