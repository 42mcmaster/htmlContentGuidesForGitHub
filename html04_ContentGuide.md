# html04 Content Guide: Photos, Promo Video, and Table

This guide goes with `html04_Project.md`. The project adds three things to your Shiny Log site. This guide tells you what the photos, the video, and the table should be about.

---

## Part 1: Photo Gallery

**Where:** a new page, `gallery.html`. Add a `Gallery` link to the nav on all pages (header and footer) so it sits between About and Contact.

**Page text:**
- `<h2>`: `Shiny Gallery`
- `<p>` under it: `Pictures of every shiny I have found, in the order I found them.`

**The photos: take screenshots of your own shinies.** These are your own pictures, so they are the best thing to use.

1. On your Switch, open the game and get the shiny on screen (the summary screen or the box works well).
2. Press the capture button (the square button on the left Joy-Con).
3. Go to the Switch home menu > Album > pick the screenshot > Sharing and Editing > Send to Smartphone. The Switch shows two QR codes: scan the first one to connect your phone to the Switch, then scan the second one to open the download page. You can send up to 10 pictures at once.
4. Get the pictures from your phone to the school computer (email them to yourself or use Google Drive).
5. Save them in your site's `images` folder with these exact names (all lowercase, no spaces):
   - `images/shiny-kricketot.jpg` (Lemon)
   - `images/shiny-skuntank.jpg`
   - `images/shiny-avalugg.jpg` (Iceberg, after evolving; or `shiny-bergmite.jpg` if you have a picture from before)
   - `images/shiny-sandile.jpg`
   - `images/shiny-jigglypuff.jpg`
   - `images/shiny-scatterbug.jpg`
   - `images/shiny-drilbur.jpg`
   You need at least 3. More is fine.

**If you cannot get screenshots off the Switch:** take a phone photo of Pokémon things you own (cards, a plush, the game case) instead. Same file naming idea: `images/card-pikachu.jpg`.

**For each photo:**
- `alt` text pattern: `Shiny [Pokémon] in Pokémon [game]` — example: `Shiny Kricketot in Pokémon Legends: Arceus`
- `width` and `height`: use `width="400"` and the matching height. Switch screenshots are 16:9 (1280 x 720, or 1920 x 1080 on Switch 2), so 400 x 225 works either way.
- `<figcaption>` pattern: `[Nickname if it has one] the shiny [Pokémon] - [game]` — example: `Lemon the shiny Kricketot - Legends: Arceus`

**Credits line** at the bottom of the gallery page, in a `<p>`:
> All screenshots were taken by me on my Nintendo Switch. Pokémon is a trademark of Nintendo, Creatures Inc., and GAME FREAK inc.

If you used a photo from Wikimedia Commons instead, credit it the way `images/CREDITS.md` shows.

---

## Part 2: Promo Video (20 seconds, Lego figures)

**The idea:** a Lego trainer has been hunting for a shiny forever. The ad says the Shiny Log is the place to keep track of hunts and see what a real find looks like.

**Characters (2 max):** a Trainer and a friend. Give them names before you write.

**Script plan.** Write your own lines. Each block has what to say and one example line to show the size.

| Seconds | What happens | Example of the size of line you need |
|---|---|---|
| 0–4 | The hook: the Trainer is tired of hunting with no luck | *"Three thousand encounters. Still no shiny."* |
| 4–14 | The friend shows the site and names 2 or 3 things on it: the list of every shiny, the gallery, and the full-odds explanation | *"Check out The Shiny Log. Every find, every game, and a gallery to prove it."* |
| 14–20 | Closing line with the site name | *"The Shiny Log. Keep hunting."* |

About 45 words total. Time it with your partner. Show Mr. McMaster the script before you record.

**Shot list.** The project wants one line per picture (40 to 60 pictures). Plan it as six scenes, then write how many pictures each scene gets (about 8 to 10 each). Scenes:
1. Trainer figure alone at a desk, head down (tired)
2. Trainer looks up
3. Friend figure walks in from the side
4. Both figures look at a "screen" (a folded piece of paper or a phone)
5. Friend points at the screen
6. Both figures face the camera for the site name (take extra pictures of this pose to hold at the end)

**Set:** a desk, plain background, one or two props. A Poké Ball drawn on paper or a small Pokémon toy works as a prop.

**Text on the last pages in Canva:** `The Shiny Log`

**File names:** the voice export from Audacity is `promo-voice-yourlastname.mp3` and the finished video is `promo-yourlastname.mp4` (put your actual last name in place of "yourlastname"). Both go in the `media` folder.

**Embed it** on `index.html` in a new section `id="promo"` with the `<h2>` `Watch the Promo`, using the `<video>` code from the project file.

---

## Part 3: Comparison Table

**Where:** on `index.html`, in the `Every Shiny So Far` section, under the list. Or make a new section `id="table"` right after it.

**What it compares:** your shiny finds. You have 7, so you have more than the 4 rows you need.

**Caption:** `My shiny finds compared by game, type, and odds`

**Header row (`<th>`):** `Pokémon` | `Nickname` | `Game` | `Type` | `Full odds?`

**Data rows:** one per shiny. Fill in from your list. For the Type column, look each Pokémon up on Bulbapedia and copy the type (some have two, like Poison/Dark). For Full odds, write `Yes` or `No (NTFO)`.

| Pokémon | Nickname | Game | Type | Full odds? |
|---|---|---|---|---|
| Kricketot | Lemon | Legends: Arceus | (look up) | No (NTFO) |
| Skuntank | none | Legends: Arceus | (look up) | No (NTFO) |
| Bergmite | Iceberg | Scarlet | (look up) | Yes |
| Sandile | none | Scarlet/Violet DLC | (look up) | Yes |
| Jigglypuff | none | Violet | (look up) | Yes |
| Scatterbug | none | Violet | (look up) | Yes |
| Drilbur | none | Legends: Z-A | (look up) | Yes |

**The colspan or rowspan:** add a title row at the very top: one `<th colspan="5">` that reads `Shiny Finds, 2022 to 2025`. Five columns below it, so colspan is 5.

---

## Done when

- [ ] `gallery.html` exists, is in the nav on every page, has 3+ screenshots with alt, width, height, figure, figcaption, and the credits line
- [ ] Script written, timed, approved; video recorded, built, exported under 10 MB, embedded on the home page
- [ ] Table on the home page with the caption, header row, 7 rows, and the colspan title row
- [ ] Validator passes, pushed with the `images` and `media` folders
