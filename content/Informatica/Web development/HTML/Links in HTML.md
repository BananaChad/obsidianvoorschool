---
title: Links in HTML
---

# Links in HTML

Met links maak je tekst klikbaar. In HTML gebruik je daarvoor het **anchor-element** (`<a>`).

## Het `a`-element

Het `a`-element heeft een `href`-attribuut: de plek waar de link naartoe gaat. De tekst tussen de openingstag en de sluitingstag is de tekst die de bezoeker ziet en kan aanklikken.

```html
<a href="https://google.com">dit is Google</a>
```

Resultaat: <a href="https://google.com">dit is Google</a>

## Een link midden in een zin

Je kunt een link ook gewoon in een alinea gebruiken:

```html
<p>Dit is <a href="https://google.com">Google</a>.</p>
```

Resultaat: <p>Dit is <a href="https://google.com">Google</a>.</p>

## Openen in een nieuw tabblad

Met `target="_blank"` opent de link in een nieuw tabblad. Dat is handig bij bijvoorbeeld social media: de bezoeker blijft op jouw website.

```html
<a href="https://instagram.com" target="_blank">Instagram</a>
```

## Toegankelijkheid: `hreflang`

Met `hreflang` vertel je de browser in welke taal de pagina achter de link is geschreven:

```html
<a href="https://example.com" hreflang="nl">Nederlandse pagina</a>
```

## Klikbare afbeeldingen

Je kunt een afbeelding klikbaar maken door het `img`-element binnen het `a`-element te zetten. Het eerste deel is de link, het tweede deel is wat je ziet.

```html
<a href="https://freecatphotoapp.com">
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="Een schattige oranje kat op zijn rug">
</a>
```

## Meer lezen

- [MDN: HTML-elementen](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) (Engels)
- Zie ook: [[Afbeeldingen in HTML]]