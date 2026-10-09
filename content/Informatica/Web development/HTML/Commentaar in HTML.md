---
publish: true
title: Commentaar in HTML
created: 2026-10-09T14:29:16.968Z
modified: 2026-10-09T12:28:46.000Z
published: 2026-10-09T12:28:46.000Z
---

# Commentaar in HTML

Een commentaar is een opmerking in je code die de browser niet laat zien. Je gebruikt commentaar bijvoorbeeld om:

- aan jezelf (of aan anderen) uit te leggen wat een stuk code doet;
- een TODO (nog te doen-werk) te noteren;
- een opdracht te geven aan een andere ontwikkelaar.

## Hoe schrijf je een commentaar?

Een commentaar begint met `<!--` en eindigt met `-->`. Alles daartussen wordt door de browser genegeerd.

```html
<!-- TODO: deze alinea is niet meer nodig, verwijder hem -->
<p>test alinea</p>
```

## Veelgemaakte fouten

1. **Verkeerde volgorde van de tekens.** Als je `-->` en `<!--` omdraait, commentarieer je per ongeluk de code die onder je commentaar staat. Die code wordt dan niet meer uitgevoerd.

```html
-->
TODO: deze alinea is niet meer nodig.
<!--
<p>test alinea</p>
```

2. **De commentaartekens helemaal vergeten.** Dan denkt de browser dat je tekst echte code is, en wordt de tekst gewoon op de pagina getoond terwijl jij een opmerking bedoelde.

## Waar gebruik je commentaar voor?

**Uitleggen wat code doet:**

```html
<!-- deze alinea legt uit wat ons bedrijf doet -->
<p>Wij bouwen treininfrastructuur, zodat je veilig met de trein kunt reizen.</p>
```

**Een opdracht geven aan een collega:**

```html
<!-- maak alsjeblieft alle knoppen oranje, ook deze! -->
<button>Klik hier</button>
```
