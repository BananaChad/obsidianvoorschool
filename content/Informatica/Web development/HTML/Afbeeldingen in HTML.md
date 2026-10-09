---
title: Afbeeldingen in HTML
---

# Afbeeldingen in HTML

## Een afbeelding toevoegen: `img`

Met het `img`-element voeg je een afbeelding toe aan je pagina. Het `src`-attribuut vertelt de browser waar de afbeelding staat:

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
```

## Alt-tekst: `alt`

Elke afbeelding hoort een `alt`-attribuut te hebben: een korte beschrijving van wat er op de afbeelding staat. Schermlezers gebruiken die tekst voor toegankelijkheid, en de tekst verschijnt ook als de afbeelding niet kan laden.

```html
<img src="kat.jpg" alt="Een kat">
```

## Bijschrift: `figure` en `figcaption`

Met `figure` groepeer je de afbeelding, en met `figcaption` geef je er een bijschrift bij:

```html
<figure>
  <img src="lasagne.jpg" alt="Een stuk lasagne op een bord">
  <figcaption>Katten zijn dol op lasagne.</figcaption>
</figure>
```

Het verschil tussen `figcaption` en een kop: het bijschrift hoort bij de afbeelding en staat er direct naast; een kop is de titel van de hele pagina of een sectie.