# html06 Content Guide: Card Page with Fixed Header and Footer

This guide goes with `html06_DIYTask.md`. That task tells you the sizes, padding, and positioning. This guide tells you what goes in the header, the cards, the sidebar, and the footer.

**The page:** a "Shiny Cards" page. Each card is one of your shiny finds.

---

## Header (fixed at the top)

- `<h1>`: `Shiny Cards`
- If you add nav links in the header (optional challenge): `Home`, `About`, `Gallery`, `Contact`, pointing at your html03 pages with relative paths, or `#` if the page is on its own.

---

## Cards (at least 3; you can do all 7)

Every card has the same three parts: a title, a description paragraph, and a button. Use `<article class="card">` for each one.

**Title (`<h3>`):** the Pokémon name, with the nickname first if it has one.
**Description (`<p>`):** two sentences. Sentence 1: which game and when in your playthrough you found it. Sentence 2: one detail (where it was, how you reacted, whether it was full odds, what it evolved into).
**Button:** `See the hunt`

Here are the titles and the facts for each card. You write the sentences.

| Card | Title | Facts to use in the description |
|---|---|---|
| 1 | `Lemon the Kricketot` | Legends: Arceus, your first playthrough, not true full odds |
| 2 | `Skuntank` | Legends: Arceus, Daybreak update, found during a massive mass outbreak, not true full odds |
| 3 | `Iceberg the Bergmite` | Scarlet playthrough, later evolved into Avalugg (say which form and which game you evolved it in) |
| 4 | `Sandile` | Scarlet/Violet DLC, The Indigo Disk |
| 5 | `Jigglypuff` | unfinished Violet playthrough |
| 6 | `Scatterbug` | unfinished Violet playthrough |
| 7 | `Drilbur` | Legends: Z-A, your newest find |

**Featured card (optional challenge):** make the Drilbur card the featured one. Give it `class="card featured"` and a different border color, and add the word `NEW` to the title.

---

## Sidebar (optional)

If you add the sidebar, put this in it:
- `<h3>`: `Games`
- `<ul>` of the games you have found shinies in: `Legends: Arceus`, `Scarlet`, `Violet`, `Scarlet/Violet DLC`, `Legends: Z-A`

---

## Footer (fixed at the bottom)

- `<p>`: `© 2026 The Shiny Log. Screenshots are my own.`

---

## Colors

Use the same Poké Ball scheme as your html05 page so everything matches:
- Header and footer background: `#222224` (dark), text white
- Card background: `#F9F9F9`
- Card border: `#E3350D` (red), 2px
- Featured card border: `#FFCB05` (yellow)
- Button background: `#3B4CCA` (blue), text white; hover: `#E3350D`

---

## Comments to include

Put a comment above the header, above the first card, and above the footer saying what each part is. Put a comment at the top of the CSS that says which rules handle the card and which handle the layout.

---

## Done when

- [ ] Header and footer are fixed, dark, with the text above
- [ ] At least 3 cards with a title, a two-sentence description, and a button
- [ ] One hover effect (the button color change counts)
- [ ] Files named `html06_DIYTask_Submission.html` and `.css`, pushed
