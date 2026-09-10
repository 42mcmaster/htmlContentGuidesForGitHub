# html08 Content Guide: Survey Form

This guide goes with `html08_DIYTask.md`. That task tells you which form elements you need and how to style them. This guide tells you what the survey asks.

**The survey: Shiny Hunter Survey.** A survey for other Pokémon players about how they shiny hunt. You could put it on your Shiny Log site later.

---

## Page top

- `<title>`: `Shiny Hunter Survey`
- `<h1>`: `Shiny Hunter Survey`
- `<p>` under it: `Tell me about your shiny hunting. It takes about two minutes.`

---

## Fieldset 1: About You

`<legend>`: `About You`

| Field | Type | Label | Placeholder | Notes |
|---|---|---|---|---|
| name | text | `Name` | `Your trainer name` | `required` |
| email | email | `Email` | `you@example.com` | `required` |
| city | text | `City` | `Where do you play?` | |
| yearsPlaying | number | `Years playing Pokémon` | `10` | `min="0" max="30"` |
| firstShinyDate | date | `Date of your first shiny` | | |

Use the field name as the `id` and `name`: `id="yearsPlaying" name="yearsPlaying"`.

---

## Fieldset 2: Your Games

`<legend>`: `Your Games`

**Checkboxes** (`name="games"`), label text: `Which games have you found a shiny in? Check all that apply.`
- `Legends: Arceus`
- `Scarlet`
- `Violet`
- `Scarlet/Violet DLC`
- `Legends: Z-A`

**Select dropdown** (`id="favoriteGen" name="favoriteGen"`), label: `Favorite generation`
- placeholder option: `Pick one` (with `value=""` and `selected disabled`)
- `Gen 1 (Red, Blue, Yellow)`
- `Gen 4 (Diamond, Pearl, Platinum)`
- `Gen 6 (X and Y)`
- `Gen 8 (Sword, Shield, Legends: Arceus)`
- `Gen 9 (Scarlet, Violet)`

---

## Fieldset 3: Shiny Hunting

`<legend>`: `Shiny Hunting`

**Radio buttons** (`name="method"`), label text: `Which hunting method do you use most?` (pick one)
- `Full odds (no boosts)`
- `Shiny Charm`
- `Masuda method (breeding)`
- `Mass outbreaks`
- `Sandwiches or other boosts`

**Second radio group** (`name="rating"`), label text: `How lucky do you think you are?`
- `1 - Not lucky at all`
- `2`
- `3`
- `4`
- `5 - Very lucky`

---

## Fieldset 4: Your Best Find

`<legend>`: `Your Best Find`

**Textarea** (`id="bestFind" name="bestFind"`, `rows="5" cols="40"`)
- Label: `Tell me about your best shiny find`
- Placeholder: `Which Pokémon, which game, and how long did it take?`

---

## Buttons

- Submit button text: `Send my answers`
- Reset button text: `Clear the form`

---

## Colors and font

Same as your other pages: page background `#F4F4F4`, form background white, legend text `#E3350D`, submit button `#3B4CCA` with white text (hover `#E3350D`), reset button gray `#888888`. Focus state on inputs: border `#FFCB05`. Font: the same Google Font you used in html05.

---

## Comments

Put a comment above each fieldset naming it: `<!-- Fieldset 1: About You -->` and so on.

---

## Done when

- [ ] 4 fieldsets with the legends above
- [ ] 3 text-type inputs (name, email, city), a number, a date
- [ ] 5 checkboxes, two radio groups of 5, a select with a placeholder and 5 options, a textarea
- [ ] Every input has a `<label for="">` that matches its `id`
- [ ] Styled, responsive at 600px, pushed in `html08_DIYTask_YourName`
