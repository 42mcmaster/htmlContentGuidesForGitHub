# html11 Content Guide: Build It Three Ways

This guide goes with the html11 unit files (`html11_ClientScenarios.md`, `html11_ProposalTemplate.md`, `html11_HandoffTemplate.md`). The unit asks you to pick a client and build the same site three ways. This guide gives you the client and the answers for the writing parts.

---

## Your client (scenario 5, set up by Mr. McMaster)

**Medina Shiny Hunters** — a Pokémon club that meets after school to trade, battle, and shiny hunt together. About 25 members. The club officer who runs the site is not a coder.

The club needs:
- a home page with **announcements** (next meeting, trade nights, cancellations)
- a **meeting and event schedule** (this is the data table)
- a **join form** (name, email, grade, favorite game, which events they want)
- a **photo gallery** of member shiny finds
- an **about page** with club rules and how full odds works
- **dark mode**, because members check the site on their phones at night while hunting

That covers everything scenario 5 requires: multiple pages, a table, a form, a gallery, and regular updates by a non-coder.

---

## 11a: The mini-proposal (ProposalTemplate blanks)

| Blank | Put this |
|---|---|
| Website name | `Medina Shiny Hunters` |
| Theme / purpose | A club website that tells members when and where the club meets, lets new people join, and shows off members' shiny finds. |
| Target audience | Students who play Pokémon, new members who want to join, and parents who want to know when meetings are. |
| Your goal | Finish this sentence: "I want to build a site the club officer can update without asking a coder, and I am most excited to build the..." |

**Sitemap (4 pages):**
- `index.html` Home: hero headline `Hunt together. Trade together.`; an Announcements section with 3 sample announcements (next meeting date, a trade night, a weather cancellation); a link to the join form.
- `about.html` About: what the club is, when it started, the club rules (use your shiny hunting rules from html03 as a start), and a short full-odds explanation.
- `events.html` Events: the **table**. Columns: `Date` | `Event` | `Room` | `Bring`. Six rows: three regular meetings, one trade night, one shiny hunt night, one tournament. A caption `Fall meeting schedule`.
- `contact.html` Join: the **form**. Fields: name (text), email (email), grade (select: 9, 10, 11, 12), favorite game (select), events you want (checkboxes: meetings, trade nights, tournaments), a message textarea. Submit button `Join the club`. Below it, the club email `shinyhunters@example.com` and the meeting room.

**Visual design blanks:** Primary `#E3350D` (red), Secondary `#3B4CCA` (blue), Accent `#FFCB05` (yellow), Neutrals `#222224` text and `#F4F4F4` background. Heading font: the Google Font you used in html05. Body font: the same font, or `Arial, sans-serif`.

**Content plan blanks:**
- Total images: 4 (three shiny screenshots from your gallery and one photo of a Pokémon card or plush for the home page hero).
- Where from: your own Switch screenshots and your own phone photos. Credit line the same as your gallery.
- Text content: the sentences you wrote for the Shiny Log, reworded so they say "the club" and "members" instead of "I". Announcements and the schedule rows are new; write them from the events table above.

**Form details:** required fields are name and email; email must look like an email; the message must be at least 20 characters (same three checks as html09). After submission: a thank-you message on the page, and in real life the server would save the answers in a database and email the club officer.

**SEO blanks (title and meta for each page):**
- Home: `Medina Shiny Hunters - Pokémon Club` / a sentence about when the club meets and how to join
- About: `About Medina Shiny Hunters` / a sentence about the club rules and full-odds hunting
- Events: `Meeting and Event Schedule - Medina Shiny Hunters` / a sentence about the fall schedule
- Join: `Join Medina Shiny Hunters` / a sentence about the sign-up form

**Responsive strategy:** mobile first, one column, the hamburger nav below 768px, two columns for the gallery at 768px and three at 1024px (what you built in html07 and html09).

**Wireframes:** draw the four pages on paper as boxes: header with nav, one main box per section listed above, footer. Take a phone picture and put it in the proposal folder, or describe each in two lines.

**Timeline and deliverables:** copy the segment order from the unit guide (11a through 11g) and put a class day next to each.

---

## 11b: The hand-coded build

This is your Shiny Log site, reworked for the club. Change the site name in the header and titles to `Medina Shiny Hunters`, swap your personal shiny list for the announcements and schedule, keep the gallery, and keep dark mode and the hamburger nav from html09.

---

## 11c: The AI build

When you direct the AI, give it the client list above word for word, plus the non-negotiables from the AI build guide (semantic HTML5, alt text on every image, external CSS). **Save the whole conversation as your prompt log**; it is a graded file.

For `html11_AICritique_YourName.md` you need at least five findings. Each finding has three parts: the line or section, what is wrong or questionable, and what you would change. Start by checking these five things, and write a finding for each one whether it passed or not:
1. Is the schedule a real `<table>` with `<th>` headers and a caption?
2. Does every form field have a `<label for="">` that matches its id?
3. Is the nav inside a `<nav>` and the page content inside `<main>`?
4. Does every image have alt text that says what is in it?
5. Is there exactly one `<h1>` on each page?

Then do the one revision round: tell the AI to fix the two worst findings, and note in the critique what changed.

---

## 11d: The builder builds (Google Sites, WordPress.com)

Same content, copied from your hand-coded build. Google Sites is the quick one: the home page and the events page only. WordPress.com gets all four pages. Put both URLs and your observations in `html11_BuilderNotes_YourName.md`. For the observations, answer three things for each builder: how long the home page took, what you could not do (a real table, a working form, dark mode), and whether the club officer could update it alone.

---

## 11f: The comparison matrix

Fill it in from your testing. For the verdict paragraph, answer in this order: which build you recommend for the club, the one reason that matters most (the officer cannot code, so updates have to be easy), and what the club gives up by choosing it.

---

## 11g: The handoff document

Use the four headings from `html11_HandoffTemplate.md`. For the three "how to update it" walk-throughs, use these:
1. Change the next meeting date on the home page
2. Add a new shiny photo to the gallery
3. Post a cancellation announcement

Write each as numbered steps for the build you recommended.

**Presentation, last item ("one thing you'd tell last-August-you"):** pick one: name files in lowercase with no spaces from day one, take screenshots early, or test on a phone before you think you are done.

---

## Done when

- [ ] Proposal filled in with the answers above
- [ ] Hand-coded and WordPress versions have all 4 pages; Google Sites has home and events; all use the same text
- [ ] Prompt log and critique with 5 findings committed
- [ ] Matrix and verdict written
- [ ] Handoff doc with the 3 update walk-throughs, pushed
