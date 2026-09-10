# html03 Content Guide: Your 3-Page Mini-Site

This guide goes with `html03_DIYTask.md`. The task tells you how to build the pages. This guide tells you what to put in them.

**Your site topic: The Shiny Log.** A website that keeps track of every shiny Pokémon you have found. You already wrote most of this content on your About Me page. Now it gets its own site.

Right now your html03 folder has the Travel Adventure sample in it. Keep the structure. Replace every piece of Travel Adventure text with the Shiny Log text below.

---

## Every page (header, nav, footer)

| Spot | Put this |
|---|---|
| `<title>` | `The Shiny Log - Home` / `The Shiny Log - About` / `The Shiny Log - Contact` |
| `<h1>` in the header | `The Shiny Log` |
| Nav links (header and footer) | `Home` → index.html, `About` → about.html, `Contact` → contact.html |
| Footer copyright | `© 2026 The Shiny Log. All rights reserved.` (use `&copy;`) |

Remember `id="top"` on the header of every page.

---

## index.html (Home)

Three sections. Each one gets an `id` so the jump links work.

**Intro paragraph (before the sections):** one sentence that says what the site is. Use this one or change a few words:
> This site is a log of every shiny Pokémon I have found since Pokémon Legends: Arceus.

**Jump links ("Jump to:")** → `#latest`, `#list`, `#odds`

**Section 1** — `id="latest"`
- `<h2>`: `Latest Shiny`
- `<p>`: two sentences about your newest find, the Drilbur from Legends: Z-A. Sentence 1: what it is and which game. Sentence 2: one detail you remember (where you were in the game, how long it took, or what you did when you saw it).

**Section 2** — `id="list"`
- `<h2>`: `Every Shiny So Far`
- `<ul>`: one `<li>` per shiny, oldest first. Write each one as **Nickname (Pokémon) - game**. Use your list from your About Me page:
  1. Lemon (Kricketot) - Legends: Arceus
  2. Skuntank - Legends: Arceus, Daybreak update
  3. Iceberg (Bergmite, now Hisuian Avalugg) - Scarlet
  4. Sandile - Scarlet/Violet DLC, The Indigo Disk
  5. Jigglypuff - Violet
  6. Scatterbug - Violet
  7. Drilbur - Legends: Z-A

**Section 3** — `id="odds"`
- `<h2>`: `What Full Odds Means`
- `<p>`: explain full odds in two or three sentences. You already wrote this on your About Me page (the 1/4096 sentence). Copy it here and add one sentence that says what NTFO means.

---

## about.html (About)

**Top of the page:**
- `<h2>`: `About This Site`
- `<p>`: two sentences. Sentence 1: why you started keeping a shiny log. Sentence 2: what you want people to get from it. If you are stuck, start with: *"I started this log because..."*

**Jump links** → `#hunter`, `#rules`, plus `Back to Home` → index.html

**Section 1** — `id="hunter"`
- `<h3>`: `About the Hunter`
- `<p>`: three sentences. (1) Your first name and that you are a student at Medina County Career Center. (2) Which Pokémon game you played first. (3) The trumpet and marching band sentence from your About Me page.
- Do not put your last name, school email, or address on this page. The site is public.

**Section 2** — `id="rules"`
- `<h3>`: `My Shiny Hunting Rules`
- `<p>`: one sentence that says you try to keep every hunt at full odds.
- `<ul>` with three rules you follow. Examples of the kind of thing to write: no Shiny Charm, no Masuda method, no outbreaks. Use your real rules.

---

## contact.html (Contact)

- `<h2>`: `Contact`
- `<p>`: `Want to share a shiny find or ask a question? Here is how to reach the log.`

**Section 1** — `id="contact-info"`
- `<h3>`: `Contact Information`
- Email link: use a fake address, because the site is public. `mailto:shinylog@example.com`, link text `Email the Shiny Log`
- Phone link: use the fake number from the task. `tel:+1-555-0100`, link text `Call the Shiny Log`

**Section 2** — `id="resources"`
- `<h3>`: `Shiny Hunting Resources`
- `<ul>` with three external links. All three need `target="_blank"`. Link text must say where the link goes (no "click here").
  1. `Bulbapedia` → https://bulbapedia.bulbagarden.net
  2. `Serebii` → https://www.serebii.net
  3. `The official Pokémon website` → https://www.pokemon.com

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
