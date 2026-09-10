# html09 Content Guide: Mad Libs Page and the Three Features

This guide goes with two task files: `html09_DIYTask.md` (Mad Libs) and `html09_FeaturesDIYTask.md` (dark mode, hamburger nav, form validation).

---

## Part A: Mad Libs Story Generator

**The story: a shiny hunt that goes wrong in a funny way.**

### Page text

- `<title>`: `Shiny Hunt Mad Libs`
- `<h1>`: `Shiny Hunt Mad Libs`
- Instructions `<p>`: `This page builds a silly shiny hunting story out of words stored in JavaScript. Reload the page or click the button to read it.`
- Output element: `<p id="storyOutput"></p>`

### The 9 variables (the task needs 8)

Give each one a real value. Pick your own words; the middle column is just the kind of word.

| Variable name | Kind of word | Example value |
|---|---|---|
| `adjective1` | adjective | `sparkly` |
| `adjective2` | adjective | `grumpy` |
| `pokemon1` | noun (a Pokémon) | `Kricketot` |
| `pokemon2` | noun (a different Pokémon) | `Skuntank` |
| `verb1` | verb | `sneeze` |
| `verb2` | verb | `dance` |
| `townName` | place | `Jubilife Village` |
| `numberOfBalls` | number | `47` |
| `moveName` | a Pokémon move | `Tackle` |

Write a comment above each one that says what it stores, like `// adjective1 describes the shiny`.

### The function

- Name: `generateShinyStory`
- Parameters: at least 4 of the variables. Use all 9 if you want the full story.
- It returns a template literal.

### The story (three sentences)

Write these in the template literal with `${ }` around each variable. Here is the story in plain words, with the variable that goes in each blank:

1. After a long day in **[townName]**, a **[adjective1]** shiny **[pokemon1]** finally showed up, and I threw **[numberOfBalls]** Poké Balls at it.
2. Right before the last ball hit, a **[adjective2]** **[pokemon2]** jumped in front of it and started to **[verb1]**.
3. The shiny used **[moveName]**, everyone started to **[verb2]**, and I still have not caught it.

You can change any of the sentences. The blanks are the part that matters.

### File names

`html09_DIYTask_YourName.html` and `html09_DIYTask_YourName.js` (external file, linked with `<script src="html09_DIYTask_YourName.js"></script>` at the end of the body).

### Display it

Call the function, store the result in `myStory`, and put it on the page with `document.getElementById('storyOutput').textContent = myStory;`. Add a comment above that line that says it puts the story on the page.

### Stretch goal (pick one)

The easiest one is **Add a Button**: `<button onclick="generateNewStory()">Tell it again</button>`. Inside `generateNewStory`, swap in a second set of words (for example `pokemon1 = 'Drilbur'`) and display it again.

---

## Part B: The three features on your real site

These go on your Shiny Log site (html03 pages plus the gallery). Most of this is code, not content. Here is the content part.

**First, move the survey into the site.** Feature 3 has to be on your real site, so copy your html08 `index.html` into the Shiny Log folder as `survey.html`, merge its CSS into the site's `styles.css`, and add a `Survey` link to the nav on every page (after Gallery). From now on the survey lives there.

### Feature 1: Dark mode

Your CSS custom properties on `:root`. Use your existing colors so the site does not change:
```
--bg: #F4F4F4;       --text: #222224;
--header: #E3350D;   --accent: #3B4CCA;   --highlight: #FFCB05;
```
The `.dark-mode` override swaps `--bg` to `#1B1B1E` and `--text` to `#F4F4F4`. Keep the red and yellow the same.

Button label text: `Dark mode` when the page is light, `Light mode` when it is dark.

### Feature 2: Hamburger nav

The button text is `☰` and it needs `aria-label="Open menu"`. No other content.

### Feature 3: Form validation (on your Shiny Hunter Survey)

The three checks and the friendly message for each. Write these messages into the page, not into `alert()`:

| Check | Message |
|---|---|
| Name is empty | `Please enter your trainer name.` |
| Email does not look like an email | `That email does not look right. Try you@example.com.` |
| Best Find textarea is shorter than 20 characters | `Tell me a little more about your best find (at least 20 characters).` |

Success message when everything passes: `Thanks! Your answers were sent.`

### The server comment at the top of script.js

The task wants two or three sentences using the words *server*, *database*, and *validation happens again on the server because users can bypass yours*. Here is the shape; write it in your own words:

> When the survey is submitted, a server would receive the answers and save them in a database. Validation happens again on the server because users can bypass yours by turning off JavaScript or editing the page.

---

## Done when

- [ ] Mad Libs page shows a three-sentence story built from 8+ variables through a function with 4+ parameters
- [ ] Dark mode button, hamburger button, and survey validation are on the real site with the text above
- [ ] One `script.js`, every function commented, server comment at the top
- [ ] Pushed
