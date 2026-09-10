# html10 Content Guide: SEO Audit and Publishing

This guide goes with `html10_SeoDIYTask.md` and `html10_PublishDIYTask.md`. Both tasks start with "choose a project." **Your project is your Shiny Log site** (the html03 pages, the gallery, and the survey). It has multiple pages, images, and a form, which is everything the tasks ask for.

Most of these two tasks are checklists and fill-in-the-blank reports. The writing parts are below with the words to use.

---

## SEO task: title tags (under 60 characters)

| Page | `<title>` |
|---|---|
| index.html | `The Shiny Log - Every Shiny Pokémon I Have Found` |
| about.html | `About The Shiny Log - Full-Odds Shiny Hunting` |
| gallery.html | `Shiny Gallery - Screenshots of My Shiny Pokémon` |
| contact.html | `Contact The Shiny Log` |
| survey.html | `Shiny Hunter Survey - The Shiny Log` |

---

## SEO task: meta descriptions (150 to 160 characters)

Home page, ready to use:
> `<meta name="description" content="A log of every shiny Pokémon I have found at full odds since Legends: Arceus, with a gallery of screenshots and a plain explanation of what full odds means.">`

For the other pages, write one sentence each using this pattern: **what the page has + one detail + what the visitor can do.** Count the characters (a search for "character counter" gives you a tool).
- About: what the site is for, that the hunts are full odds, and that the rules are listed.
- Gallery: screenshots of each shiny, taken on Switch, from Legends: Arceus to Legends: Z-A.
- Contact: how to send a shiny find or a question, plus links to Bulbapedia and Serebii.

---

## SEO task: alt text

Every image already has alt text from html04. Check each one against the rule: it says what is in the picture, and it is under 125 characters. `Shiny Kricketot in Pokémon Legends: Arceus` passes. `image1` fails.

---

## SEO task: headings

Each page should have exactly one `<h1>` (the site name in the header). Section titles are `<h2>`, and the sub-sections on the About and Contact pages are `<h3>`. That is already how the html03 guide set it up, so this should pass. If the validator or WAVE says a heading level is skipped, that is the thing to fix.

---

## SEO task: AUDIT_REPORT.md

The report is a template you fill in. Use the template's headings exactly. For each issue you find, fill in the four lines the template has:
- **Location:** which file and where (example: `about.html, head`)
- **Problem:** what was wrong (example: `no meta description`)
- **Fix:** what you changed (example: `added a meta description tag`)
- **Status:** `Fixed`

**Example Fixes section:** the template wants before-and-after code. Use your first two fixes. Paste the old line under **Before** and the new line under **After** (a `<title>` fix and a meta description fix are the easiest to show).

**Testing Done:** check off WAVE, keyboard-only navigation, color contrast, and Lighthouse (PageSpeed Insights) as you do each one.

For the Notes section at the end, write two sentences: one thing the audit tools caught that you did not expect, and one thing that was already fine.

---

## Publish task: the project selection blanks

- **Project Name:** `The Shiny Log`
- **Main file:** `index.html`
- **List all files:** index.html, about.html, gallery.html, contact.html, survey.html, styles.css, script.js, the `images` folder, the `media` folder

---

## Publish task: the reflection questions

Each one wants a few sentences. Finish these:

- **What went well:** "The navigation worked on every page because..." / "The images all loaded because the file names..." / "The validator passed on the first try for..."
- **What you learned:** "The most important thing I learned was..." (pick one: how GitHub Pages turns a repo into a live site, why file names have to match exactly, or why meta descriptions matter)
- **How to improve:** "Next time I would..." (pick one: take the screenshots earlier, keep the CSS in one file from the start, or test on a phone sooner)

---

## Done when

- [ ] Every page has the title and a meta description from above
- [ ] AUDIT_REPORT.md filled in with the issues, fixes, and status
- [ ] Site live on GitHub Pages; the URL is in the publish report
- [ ] Reflection answers written
