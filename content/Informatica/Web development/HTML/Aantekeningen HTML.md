---
publish: true
title: Aantekeningen HTML
created: 2026-10-09T14:29:16.953Z
modified: 2026-10-09T12:28:46.000Z
published: 2026-10-09T12:28:46.000Z
---

# Aantekeningen HTML

Losse aantekeningen die ik tijdens de cursus heb gemaakt. Alle onderwerpen staan ook netjes uitgewerkt op de [[Web development/HTML/|HTML-overzichtspagina]].

## `figure` en `figcaption`

Met het `figure`-element groepeer je zelfstandige inhoud, zoals een afbeelding, en koppel je er een bijschrift aan:

```html
<figure>
  <img src="hond.jpg" alt="Een hond">
  <figcaption>Dit is mijn hond.</figcaption>
</figure>
```

Het verschil met een kop (`header`): een `figcaption` hoort bij de afbeelding zelf en staat er direct naast; een header is de titel van de hele pagina of sectie.

## Het anchor-element (`a`)

Eerst snapte ik niet wat een anker is: een link is onzichtbaar totdat je er tekst tussen zet.

```html
<a href="https://freecodecamp.org">Klik hier om naar freeCodeCamp te gaan</a>
```

De tekst tussen de openingstag en de sluitingstag is de tekst die de bezoeker ziet. Zonder tekst is de link onzichtbaar:

```html
<!-- dit is een onzichtbare link, want er staat geen tekst tussen de tags -->
<a href="https://freecodecamp.org"></a>
```

Het werkt dus een beetje als een backlink in Obsidian, maar dan op een website: je klikt op tekst en komt op een andere pagina terecht.
