# De Bosavonturiers

Een 2D platformspel (zoals Mario) in een groot bos, met **Emma, Thijs en Hugo** die moeten samenwerken. Alles zit in één bestand: `index.html` — geen build, geen dependencies.

## Spelen

Open `index.html` in een browser (dubbelklikken werkt). Op telefoon of tablet verschijnen er automatisch schermknoppen (multi-touch werkt); speel het liefst in liggende stand.

Doel: bereik **samen** de Gouden Boom aan het einde van het level — het poortje gaat pas open als alle drie de figuurtjes erop staan.

## Bediening

| Actie | Toetsenbord | Touch |
|---|---|---|
| Lopen | ← → of A / D | ◀ ▶ |
| Springen | Spatie / ↑ / W | SPRING |
| Hout pakken / neerleggen als brug | E | HOUT |
| Hout laten vallen (brug naar beneden) | S / ↓ | VAL |
| Teamgenoot gooien over muur/gat | F | GOOI |
| Wissel van figuurtje | 1 / 2 / 3 of Tab | WISSEL |
| Opnieuw / volgend level | R | — |

## Samenwerken

- **Spinnen** verslaan door erop te springen (net als Mario) — van opzij raken kost een hartje.
- **Grote gaten** overbrug je door stukken hout neer te leggen als planken.
- **Hoge muren** kom je over door een teamgenoot te gooien.
- Vanaf een hoge richel kun je hout **naar beneden laten vallen** om in de kuil een loopbrug te maken voor de anderen.
- Emma springt het hoogst, Thijs rent het snelst, Hugo gooit het verst.

## Meerdere levels toevoegen

In `index.html` staat bovenaan de lijst `LEVELS`. Voeg gewoon een item toe:

```js
{name:'Level 2 — De IJsgrot', build(){
  // hier zet je de bodem, platformen, hout, spinnen en de exit neer
  // (zie level 1 als voorbeeld)
}},
```

Na het winnen van een level kun je met **R** door naar het volgende level.
