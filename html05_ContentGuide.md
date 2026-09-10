# html05 Content Guide: Restyle Your About Me Page

This guide goes with `html05_DIYTask.md`. That task is about CSS, but your `aboutMe.html` has two empty spots that need content first, and it needs a few classes and ids for the CSS to hook on to. This guide covers both.

---

## Step 1: Fill the empty spots in aboutMe.html

Your page has an empty `<h3>` and `<p>` under **My Interests**. Fill them in, and add a second one:

**Interest 1**
- `<h3>`: `Shiny Hunting`
- `<p>`: two sentences. (1) What shiny hunting is, in your own words (a shiny is a rare different-colored Pokémon). (2) Which game you are hunting in right now.

**Interest 2**
- `<h3>`: `Marching Band`
- `<p>`: two sentences. (1) What you play and how long. (2) One thing you like about being in the band (the shows, the trips, the people, the music).

---

## Step 2: Add the hooks the CSS needs

The task needs 2 class selectors and 1 ID selector. Add these to your HTML (this is structure, not styling, so it is allowed):

| Add this | Where |
|---|---|
| `<div id="header">` ... `</div>` | wrap the `<h1>` with your name |
| `class="intro"` | on the first paragraph under About Me (the trumpet sentence) |
| `class="highlight"` | on the Fun Fact paragraph (the full-odds one) |
| `<div id="footer"><p>© 2026 Your Name. All rights reserved.</p></div>` | at the bottom of the body |

---

## Step 3: Pick your colors

Use a Poké Ball color scheme. These are real hex codes, ready to paste:

| Use for | Color | Code |
|---|---|---|
| Header and footer background | Poké Ball red | `#E3350D` |
| Page background | light gray | `#F4F4F4` |
| Body text | almost black | `#222224` |
| Highlight box background | Pokémon yellow | `#FFCB05` |
| Border under headings | blue | `#3B4CCA` |
| One rgb() color (the task wants at least one) | white text in the header | `rgb(255, 255, 255)` |

If you would rather use the colors of one of your shinies, pick one, look at your screenshot, and use an online color picker to get 3 hex codes from it.

---

## Step 4: Pick a font

Go to fonts.google.com and use one of these. Copy the `<link>` tag Google gives you into the `<head>`.
- `Nunito` (round and friendly)
- `Poppins` (clean)
- `Press Start 2P` (looks like an old game; use it for the `h1` only, it is hard to read in paragraphs)

---

## Step 5: Your 10 CSS rules

Here is a list of 10 rules that hits every requirement. You write the properties inside each one.

| # | Selector | Kind | Put at least this in it |
|---|---|---|---|
| 1 | `body` | element | font-family (your Google Font), background-color, color, line-height |
| 2 | `h1` | element | font-size, text-align: center, letter-spacing |
| 3 | `h2` | element | color, border-bottom, padding-bottom |
| 4 | `h3` | element | color, font-size |
| 5 | `p` | element | font-size, margin-bottom |
| 6 | `li` | element | margin-bottom |
| 7 | `.intro` | class | font-size (bigger), font-style: italic |
| 8 | `.highlight` | class | background-color (yellow), padding, border-left, font-weight: bold |
| 9 | `#header` | id | background-color (red), color (the rgb white), padding, text-align: center |
| 10 | `#footer` | id | background-color, color, text-align: center, padding, margin-top |

That gives you 6 element selectors, 2 class selectors, 2 ID selectors, 3+ hex colors, 1 rgb color, and fonts and text properties. Add `text-decoration` somewhere (for example `text-decoration: underline` on `h2`) so all three text properties on the checklist are covered.

---

## Done when

- [ ] My Interests has two `<h3>` + `<p>` pairs with real sentences
- [ ] `#header`, `#footer`, `.intro`, `.highlight` are in the HTML
- [ ] `styles.css` is linked and has the 10 rules above
- [ ] Google Font loads
- [ ] Both files pushed
