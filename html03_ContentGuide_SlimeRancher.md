# html03 Content Guide: Your 3-Page Mini-Site

This guide goes with `html03_DIYTask.md`. The task tells you how to build the pages. This guide tells you what to put in them.

**Your site topic: The Slime Ranch Log.** A website about the slimes on your ranch in Slime Rancher (or Slime Rancher 2): which slimes you keep, what they eat, and how you run your ranch.

Right now your html03 folder has the Travel Adventure sample in it. Keep the structure. Replace every piece of Travel Adventure text with the Slime Ranch Log text below.

---

## Every page (header, nav, footer)

| Spot | Put this |
|---|---|
| `<title>` | `The Slime Ranch Log - Home` / `The Slime Ranch Log - About` / `The Slime Ranch Log - Contact` |
| `<h1>` in the header | `The Slime Ranch Log` |
| Nav links (header and footer) | `Home` → index.html, `About` → about.html, `Contact` → contact.html |
| Footer copyright | `© 2026 The Slime Ranch Log. All rights reserved.` (use `&copy;`) |

Remember `id="top"` on the header of every page.

---

## index.html (Home)

Three sections. Each one gets an `id` so the jump links work.

**Intro paragraph (before the sections):** one sentence that says what the site is. Use this one or change a few words:
> This site is a log of the slimes I raise on my ranch in Slime Rancher.

**Jump links ("Jump to:")** → `#newest`, `#list`, `#largos`

**Section 1** — `id="newest"`
- `<h2>`: `Newest Slime`
- `<p>`: two sentences about the newest slime you added to your ranch. Sentence 1: which slime it is and where you found it. Sentence 2: one detail you remember (how you caught it, what it eats, or what went wrong the first time you kept one).

**Section 2** — `id="list"`
- `<h2>`: `Every Slime on My Ranch`
- `<ul>`: one `<li>` per slime type, in the order you got them. Write each one as **Slime name - where you found it**. The list below is only an example from Slime Rancher 1. Replace it with the slimes you actually have. (If you play Slime Rancher 2, your places will be different, like Rainbow Fields or Ember Valley.)
  1. Pink Slime - The Ranch
  2. Rock Slime - The Dry Reef
  3. Tabby Slime - The Dry Reef
  4. Phosphor Slime - The Dry Reef, at night
  5. Honey Slime - The Moss Blanket
  6. Hunter Slime - The Moss Blanket
  7. Rad Slime - The Indigo Quarry

**Section 3** — `id="largos"`
- `<h2>`: `What a Largo Is`
- `<p>`: explain what a largo is in two or three sentences. Then add one sentence that says what a Tarr is. If you are stuck, start with: *"A largo is..."*

---

## about.html (About)

**Top of the page:**
- `<h2>`: `About This Site`
- `<p>`: two sentences. Sentence 1: why you started keeping a slime ranch log. Sentence 2: what you want people to get from it. If you are stuck, start with: *"I started this log because..."*

**Jump links** → `#rancher`, `#rules`, plus `Back to Home` → index.html

**Section 1** — `id="rancher"`
- `<h3>`: `About the Rancher`
- `<p>`: three sentences. (1) Your first name and that you are a student at Medina County Career Center. (2) Which Slime Rancher game you played first and what you play it on (PC, Xbox, PlayStation, or Switch). (3) One thing you like to do when you are not playing games.
- Do not put your last name, school email, or address on this page. The site is public.

**Section 2** — `id="rules"`
- `<h3>`: `How I Run My Ranch`
- `<p>`: one sentence that says how you like to keep your ranch (for example: neat and simple, full of largos, or set up to make as many Newbucks as possible).
- `<ul>` with three rules you follow. Examples of the kind of thing to write: never let a largo eat a third kind of plort, keep Boom slimes in a corral by themselves, only sell plorts when the price is high. Use your real rules.

---

## contact.html (Contact)

- `<h2>`: `Contact`
- `<p>`: `Want to share a slime tip or ask a question? Here is how to reach the log.`

**Section 1** — `id="contact-info"`
- `<h3>`: `Contact Information`
- Email link: use a fake address, because the site is public. `mailto:slimeranchlog@example.com`, link text `Email the Slime Ranch Log`
- Phone link: use the fake number from the task. `tel:+1-555-0100`, link text `Call the Slime Ranch Log`

**Section 2** — `id="resources"`
- `<h3>`: `Slime Rancher Resources`
- `<ul>` with three external links. All three need `target="_blank"`. Link text must say where the link goes (no "click here").
  1. `Slime Rancher Wiki` → https://slimerancher.wiki.gg
  2. `The official Slime Rancher website` → https://www.slimerancher.com
  3. `Monomi Park, the company that makes Slime Rancher` → https://www.monomipark.com

**Jump links at the bottom of main** → `#contact-info`, `#resources`, `Back to Home`

---

## Comments to add

The task wants a few explanatory comments. Put one above each of these:
- the header nav: `<!-- Main navigation, same on every page -->`
- the jump links: `<!-- Jump links to sections on this page -->`
- the external links: `<!-- Outside links open in a new tab -->`

---

## Done when

- [ ] No Travel Adventure text is left anywhere
- [ ] Home has 3 sections with ids and 3 jump links that work
- [ ] About has 2 sections and jump links
- [ ] Contact has the email link, the phone link, and 3 external links with `target="_blank"`
- [ ] Footer and nav match on all 3 pages
- [ ] Pushed to GitHub
