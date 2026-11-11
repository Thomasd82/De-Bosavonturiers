# De Bosavonturiers

Een 2D co-op platformspel (zoals Mario) met **Emma, Thijs en Hugo**, in één los bestand: `index.html` — geen build, geen dependencies. Open het in een browser (werkt ook op telefoon/tablet met automatische touch-knoppen).

## Het avontuur

4 gebieden × 15 levels = **60 levels**: 🌲 Het Bos · 🏙️ De Stad · 🏖️ De Duinen · 🏡 Het Dorp. Levels worden per gebied automatisch gegenereerd (met oplopende moeilijkheid). Na elk level verschijnt een **kaart** waarop je ziet welk level je nu speelt, en je voortgang wordt **opgeslagen** (localStorage) — ook handmatig met **P**.

Doel per level: bereik **samen** het doel aan het einde (alle drie de figuurtjes erop staan).

## De drie helden

- **Emma** — blond meisje, springt het hoogst
- **Thijs** — jongen met bruin bloempotkapsel, rent het snelst
- **Hugo** — jongen met blond stekeltjeshaar, gooit het verst

Wissel met **1 / 2 / 3** of **Tab** (touch: WISSEL).

## Samenwerken

- **Hout** pakken met **E** en neerleggen als brug over gaten; met **S** van een richel naar beneden laten vallen (brug in de kuil)
- **F** = gooi een teamgenoot over een hoge muur of gat
- Spring **op** enge dieren om ze te verslaan

## Dieren in het spel

Enge tegenstanders (pletten door erop te springen, van opzij raken kost een hartje): **spinnen, marters, ratten, muizen**.

Hulprix die je helpen:

- 🐴 **Paard** — spring vanaf zijn rug voor een **MEGA sprong**
- 🐐 **Geit** — springt op en neer; spring op haar rug om **hoger te stuiteren**
- 🐑 **Schaap** — eet **hoog gras** op, waardoor een pad vrijkomt
- 🐄 **Koe** — doet af en toe een **poepje**; enge dieren mijden de poep

## Bediening

| Actie | Toetsenbord | Touch |
|---|---|---|
| Lopen | ← → of A / D | ◀ ▶ |
| Springen | Spatie / ↑ / W | SPRING |
| Hout pakken / neerleggen | E | HOUT |
| Hout laten vallen | S / ↓ | VAL |
| Gooien | F | GOOI |
| Wissel figuurtje | 1 / 2 / 3 of Tab | WISSEL |
| Opslaan | P | — |
| Opnieuw / verder (op kaart) / nieuw spel | R / N | tik |

## Levels/gebieden aanpassen

In `index.html`: de lijst `AREAS` (4 gebieden met thema, vijanden en exit-stijl) en `genLevel(areaIdx, levelNum)` (level-generator). Een eigen level met de hand? Vul zelf de arrays `solids/logs/enemies/friendlies/exit`.
