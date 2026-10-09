---
title: Secties en lijsten
---

# Secties en lijsten

## Code indelen met `section`

Met het `section`-element deel je code in, zodat elementen elkaar niet in de weg zitten en je code overzichtelijk blijft:

```html
<h1>hallo</h1>
<section>
  <h2>hi</h2>
</section>
```

## Lijsten maken

Een ongeordende lijst (met opsommingstekens) maak je met het `ul`-element (unordered list), met daarin `li`-elementen voor elk item:

```html
<ul>
  <li>melk</li>
  <li>kaas</li>
</ul>
```

Een geordende lijst maak je met `ol` (ordered list). Het verschil tussen de twee:

| Ongeordende lijst (`ul`) | Geordende lijst (`ol`) |
| --- | --- |
| • eten | 1. eten |
| • drinken | 2. drinken |

Bij een ongeordende lijst staat geen nummer, omdat de volgorde er niet toe doet. Bij een geordende lijst wel.

## Een geordende lijst binnen een ongeordende lijst

Je kunt lijsten combineren door een `ol` binnen een `li` te zetten. Let op waar de sluitingstag `</li>` staat:

```html
<ul>
  <li>eerste item</li>
  <li>
    tweede item
    <!-- let op: de sluitingstag </li> staat hier nog niet -->
    <ol>
      <li>tweede item, eerste subitem</li>
      <li>tweede item, tweede subitem</li>
      <li>tweede item, derde subitem</li>
    </ol>
    <!-- hier komt de sluitingstag </li> -->
  </li>
  <li>derde item</li>
</ul>
```

Meer voorbeelden en opties: [MDN-documentatie over `ul`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul).