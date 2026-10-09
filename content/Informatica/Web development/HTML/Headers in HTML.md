---
publish: true
title: Headers in HTML
created: 2026-10-09T14:29:16.919Z
modified: 2026-10-09T12:28:46.000Z
published: 2026-10-09T12:28:46.000Z
---

# Headers in HTML

Headers (koppen) gebruik je voor grote, dikke tekst op je website. Zo is in een presentatie de titel ook groter dan de rest van de tekst.

```html
<html>
  <body>
    <h1>grote tekst</h1>
    <p>lorem ipsum bla bla bla</p>
  </body>
</html>
```

## Zes niveaus: `h1` tot en met `h6`

Er zijn zes koppen-niveaus, van groot naar klein. Hoe hoger het nummer, hoe kleiner de tekst.

```html
<html>
  <body>
    <h1>grote tekst</h1>
    <h2>steeds</h2>
    <h3>kleiner</h3>
    <h4>totdat</h4>
    <h5>het</h5>
    <h6>helemaal klein is</h6>
    <p>Lorem ipsum</p>
  </body>
</html>
```

> [!tip] Let op
> Gebruik per pagina maar één `<h1>`: dat is de titel van de hele pagina. De niveaus `h2` tot en met `h6` gebruik je voor de onderdelen daarna. Dan blijft de structuur van je pagina logisch.

Zie ook: [[Voorbeeld met headers]]
