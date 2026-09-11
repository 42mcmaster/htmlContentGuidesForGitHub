# html04 Content Guide: Photos, Promo Video, and Table

This guide goes with `html04_Project.md`. The project adds three things to your Slime Ranch Log site. This guide tells you what the photos, the video, and the table should be about.

---

## Part 1: Photo Gallery

**Where:** a new page, `gallery.html`. Add a `Gallery` link to the nav on all pages (header and footer) so it sits between About and Contact.

**Page text:**
- `<h2>`: `Ranch Gallery`
- `<p>` under it: `Pictures of the slimes on my ranch.`

**The photos: take screenshots of your own ranch.** These are your own pictures, so they are the best thing to use.

1. Open the game and get the slime on screen. A corral works well. Move close so the slime fills most of the picture.
2. Take the screenshot. How you do it depends on what you play on:

   | What you play on | How to take the screenshot | How to get it onto your phone or computer |
   |---|---|---|
   | PC (Steam) | Press `F12` | In Steam, go to View > Screenshots. |
   | PC (Xbox app or Microsoft Store) | Press `Windows key + Alt + Print Screen` | It saves in your Videos > Captures folder. |
   | Xbox | Press the Share button on the controller | Open the Xbox app on your phone, go to your captures, and save the picture. |
   | PlayStation 5 | Press the Create button, then pick Take Screenshot | Open the PlayStation App on your phone and find it under game captures. (Auto-upload has to be turned on in the PS5 settings.) |
   | Switch | Press the capture button (the square button on the left Joy-Con) | Home menu > Album > pick the screenshot > Sharing and Editing > Send to Smartphone. Scan the first QR code to connect your phone, then the second one to open the download page. |

3. Get the pictures to the school computer (email them to yourself or use Google Drive).
4. Save them in your site's `images` folder. Use this naming pattern (all lowercase, no spaces), and name them after the slimes you actually have:
   - `images/slime-pink.jpg`
   - `images/slime-rock.jpg`
   - `images/slime-tabby.jpg`
   - `images/slime-honey.jpg`
   - `images/largo-pink-rock.jpg` (for a largo, put both slime names)
   - `images/ranch-overview.jpg` (a wide picture of your whole ranch)

   You need at least 3. More is fine.

**If you cannot get screenshots:** take a phone photo of Slime Rancher things you own (a plush, a shirt, a drawing of a slime you made) instead. Same file naming idea: `images/plush-pink-slime.jpg`.

**For each photo:**
- `alt` text pattern: `[Slime] slime in Slime Rancher` — example: `Rock slime in Slime Rancher`. If you play the second game, write `Slime Rancher 2`.
- `width` and `height`: use `width="400"` and the matching height. Most game screenshots are 16:9 (1280 x 720 or 1920 x 1080), so 400 x 225 works. If your picture is a different shape, check its real size (right-click the file > Properties > Details) and ask Mr. McMaster.
- `<figcaption>` pattern: `[Slime] slime - [where it lives on my ranch]` — example: `Rock slime - my second corral`

**Credits line** at the bottom of the gallery page, in a `<p>`:
> All screenshots were taken by me in Slime Rancher. Slime Rancher is made by Monomi Park.

If you used a photo from Wikimedia Commons instead, credit it the way `images/CREDITS.md` shows.

---

## Part 2: Promo Video (20 seconds, Lego figures)

**The idea:** a Lego rancher's corral keeps getting ruined by Tarr. The ad says the Slime Ranch Log is the place to learn which slimes to keep, what they eat, and how to make largos without making Tarr.

**Characters (2 max):** a Rancher and a friend. Give them names before you write.

**Script plan.** Write your own lines. Each block has what to say and one example line to show the size.

| Seconds | What happens | Example of the size of line you need |
|---|---|---|
| 0–4 | The hook: the Rancher's corral just filled up with Tarr again | *"My whole corral just turned into Tarr."* |
| 4–14 | The friend shows the site and names 2 or 3 things on it: the list of every slime, the gallery, and the largo explanation | *"Check out The Slime Ranch Log. Every slime, what it eats, and how largos work."* |
| 14–20 | Closing line with the site name | *"The Slime Ranch Log. Keep ranching."* |

About 45 words total. Time it with your partner. Show Mr. McMaster the script before you record.

**Shot list.** The project wants one line per picture (40 to 60 pictures). Plan it as six scenes, then write how many pictures each scene gets (about 8 to 10 each). Scenes:
1. Rancher figure alone by the corral fence, head down (upset)
2. Rancher looks up
3. Friend figure walks in from the side
4. Both figures look at a "screen" (a folded piece of paper or a phone)
5. Friend points at the screen
6. Both figures face the camera for the site name (take extra pictures of this pose to hold at the end)

**Set:** a corral (Lego fence pieces or popsicle sticks), plain background, one or two props. A slime made from Play-Doh or a pink paper circle works as a prop.

**Text on the last pages in Canva:** `The Slime Ranch Log`

**File names:** the voice export from Audacity is `promo-voice-yourlastname.mp3` and the finished video is `promo-yourlastname.mp4` (put your actual last name in place of "yourlastname"). Both go in the `media` folder.

**Embed it** on `index.html` in a new section `id="promo"` with the `<h2>` `Watch the Promo`, using the `<video>` code from the project file.

---

## Part 3: Comparison Table

**Where:** on `index.html`, in the `Every Slime on My Ranch` section, under the list. Or make a new section `id="table"` right after it.

**What it compares:** the slimes on your ranch. You need at least 4 rows. Use one row for each slime type on your list.

**Caption:** `The slimes on my ranch compared by diet, favorite food, and where I found them`

**Header row (`<th>`):** `Slime` | `Diet` | `Favorite food` | `Where I found it` | `Made a largo?`

**Data rows:** one per slime. The rows below match the example list from html03. Change them to match your own list.
- **Diet:** filled in for the example slimes. If you add a slime that is not here, look it up on the Slime Rancher Wiki.
- **Favorite food:** look each slime up on the Slime Rancher Wiki and copy its favorite food.
- **Where I found it:** copy from your list.
- **Made a largo?:** write `Yes` or `No` from your own game.

| Slime | Diet | Favorite food | Where I found it | Made a largo? |
|---|---|---|---|---|
| Pink | Everything | (look up) | The Ranch | (your answer) |
| Rock | Veggies | (look up) | The Dry Reef | (your answer) |
| Tabby | Meat | (look up) | The Dry Reef | (your answer) |
| Phosphor | Fruit | (look up) | The Dry Reef | (your answer) |
| Honey | Fruit | (look up) | The Moss Blanket | (your answer) |
| Hunter | Meat | (look up) | The Moss Blanket | (your answer) |
| Rad | Veggies | (look up) | The Indigo Quarry | (your answer) |

**The colspan or rowspan:** add a title row at the very top: one `<th colspan="5">` that reads `Slimes on My Ranch`. Five columns below it, so colspan is 5.

---

## Done when

- [ ] `gallery.html` exists, is in the nav on every page, has 3+ screenshots with alt, width, height, figure, figcaption, and the credits line
- [ ] Script written, timed, approved; video recorded, built, exported under 10 MB, embedded on the home page
- [ ] Table on the home page with the caption, header row, at least 4 slime rows, and the colspan title row
- [ ] Validator passes, pushed with the `images` and `media` folders
