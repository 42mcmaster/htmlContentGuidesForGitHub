# html07 Content Guide: Responsive Photo Gallery

This guide goes with `html07_DIYTask.md`. That task tells you how to build the flexbox or grid layout and the media queries. This guide tells you what the gallery is about and what every caption says.

**The gallery:** your shiny screenshots, one card per picture. You already have the screenshots from html04. Copy the `images` folder into your `html07_DIYTask_YourName` folder.

---

## Header

- `<title>`: `Shiny Gallery - The Shiny Log`
- `<h1>`: `Shiny Gallery`
- `<p>` subtitle: `Every shiny Pokémon I have found, from Legends: Arceus to Legends: Z-A.`

---

## The photos (at least 6)

You have 7 shinies, so you have enough. If you want more pictures, add a second screenshot of one Pokémon after it evolved (for example Iceberg as Bergmite and again as Hisuian Avalugg).

Each photo card has an image and a caption. Use this pattern for all of them:

| File | `alt` text | Caption (`<p class="caption">`) |
|---|---|---|
| shiny-kricketot.jpg | `Shiny Kricketot in Pokémon Legends: Arceus` | `Lemon - Legends: Arceus` |
| shiny-skuntank.jpg | `Shiny Skuntank in Pokémon Legends: Arceus` | `Skuntank - Legends: Arceus` |
| shiny-avalugg.jpg | `Shiny Avalugg, evolved from my shiny Bergmite` | `Iceberg - Scarlet` |
| shiny-sandile.jpg | `Shiny Sandile in Pokémon Scarlet and Violet DLC` | `Sandile - The Indigo Disk` |
| shiny-jigglypuff.jpg | `Shiny Jigglypuff in Pokémon Violet` | `Jigglypuff - Violet` |
| shiny-scatterbug.jpg | `Shiny Scatterbug in Pokémon Violet` | `Scatterbug - Violet` |
| shiny-drilbur.jpg | `Shiny Drilbur in Pokémon Legends: Z-A` | `Drilbur - Legends: Z-A` |

---

## Filter buttons (optional, in the `<nav class="filters">`)

If you include the filter nav, the buttons are: `All`, `Legends: Arceus`, `Scarlet & Violet`, `Legends: Z-A`. Making them actually filter needs JavaScript, which comes later. For now they can just be styled buttons.

---

## The two extra features (the task needs at least 2)

Pick these two. Both are CSS only:
1. **Photo hover effect:** the card lifts and gets a shadow, or the image gets a little bigger (`transform: scale(1.05)`).
2. **Animated transitions:** add `transition` to the card so the hover effect fades in instead of snapping.

---

## Colors

Same Poké Ball scheme as before so your pages match: page background `#F4F4F4`, header and footer `#222224` with white text, card background `#FFFFFF`, accent (borders, caption text) `#E3350D`.

---

## Footer

- `<p>`: `© 2026 The Shiny Log. All screenshots taken by me on Nintendo Switch. Pokémon is a trademark of Nintendo, Creatures Inc., and GAME FREAK inc.`
- `<p>`: `Contact: ` followed by an email link to `shinylog@example.com` (the task wants contact info in the footer; keep using the fake address).

---

## template.html

The task asks you to save a bare skeleton as `template.html`. It is your page with the header, nav, main, and footer left in and all the gallery cards taken out. Change the `<h1>` to `Page Title` so it is clearly a template.

---

## README.md

The task wants a short README. Write one short paragraph or a few lines for each heading. Finish these sentences with your own words:

- **Layout approach:** "I used [Flexbox / Grid] because..."
- **Color scheme:** "The colors are based on a Poké Ball: red, white, and dark gray, with yellow as an accent."
- **Features implemented:** "Hover lift with a shadow, and transitions so the hover fades in."
- **Challenges:** "The hardest part was ... I fixed it by ..."
- **Browser compatibility:** "Tested in Chrome at 375px, 768px, and 1024px wide."

---

## Done when

- [ ] 6 or more photo cards with the alt text and captions above
- [ ] 1 column on phone, 2 on tablet, 3 on desktop
- [ ] Hover effect and transition work
- [ ] `template.html`, `README.md`, `index.html`, `styles.css`, and `images` all in the folder, pushed
