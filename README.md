# OMNISCIÁ website

Static site: `index.html` + `img/` (no build step, nothing to install).

## Netlify — drag & drop (fastest, ~1 minute)
1. Go to https://app.netlify.com/drop and sign in.
2. Unzip this package, then drag the **folder** (the one containing index.html) onto the page.
3. To replace an existing site (e.g. empressdiaries or a new one): Site → Deploys → drag the folder onto "Drag and drop your site output folder here".

## GitHub Pages
1. Create a new repository on github.com (e.g. `omniscia`).
2. Upload all files (index.html, img/, netlify.toml, .nojekyll) via "Add file → Upload files" and commit.
3. Settings → Pages → Source: "Deploy from a branch" → Branch: main, folder: / (root) → Save.
4. Live at https://YOUR-USERNAME.github.io/omniscia/ in a minute or two.

## GitHub + Netlify (auto-deploys on every change)
1. Do the GitHub upload above.
2. Netlify → Add new site → Import from Git → choose the repo. Build command: leave empty. Publish directory: `.`
3. Deploy.

## Editing
- Links and text live in `index.html` (search for `href=`).
- Photo order and each scene's colours are in the `.scene` blocks and the "palette per scene" CSS.

## Structure
- `/` the OMNISCIÁ landing page (this design)
- `/diaries/` the whole Empress Diaries site: home, `lounge/`, `ready/`, `oracle/`, `author/`, `flight777/`, reels in `videos/`, music in `music/`
- `/books/` the author + bookshop site (formerly omnisciabookslimited)
- Everything is self-contained. The only outside links are Gumroad, TikTok, YouTube, Instagram and news/Bible sources.

## Hosting that does not expire
GitHub Pages (free): create a repo, upload the unzipped files (on a phone, use the desktop-site mode of github.com, or the GitHub app is not needed with Add file -> Upload files), then Settings -> Pages -> main / root.
Cloudflare Pages (free): Workers & Pages -> Create -> Pages -> Upload assets -> upload this zip or folder.
Netlify Drop also works: app.netlify.com/drop.

## Coffee payment + thank-you pack
- The "Let's talk over coffee" button on the landing page opens PayPal for $7.77 (merchant ID H8Q95E9YJLZJG).
- After paying, PayPal returns the buyer to `thank-you-k7x9q2/`: the Takeaways & Revelations PDF, six flipbooks and nine sketchnotes.
- Turn on Auto Return in PayPal (Profile -> Website payments -> Website preferences -> Auto return = On, Return URL = your-site/thank-you-k7x9q2/) so buyers are sent back automatically instead of tapping "Return to merchant".
- The pack folder is not linked from anywhere else and is set to noindex, but it is a static page: anyone who knows its address can open it. To rename the folder, rename `thank-you-k7x9q2` and the same text in index.html.

## Nov 21 update
- `/heaven-sent-christmas/`: the Christmas bundle page (offer ends December 21, 2026, live countdown). The landing page ENTER button and the Rooms list both open it. Checkout is still the Gumroad bundle ($77.70) with each book's own Gumroad link.
- `/diaries/oracle/`: now GODLIKE INTELLIGENCE. Its READ tab holds the full Godlike Intelligence app (`/diaries/oracle/read/`, also opens full screen). Decks, Spreads, Combine, Astrology, MBTI, Bible, News and Journal tabs are unchanged.
- Landing page Contact: "Email me" opens a compose form (To, Subject, Message, attachments: PDF, JPG, PNG, video up to 25 MB each). Edit the address in `index.html` (search `sacredscript777`).
- `assets/omniscia.css` + `assets/omniscia.js`: the landing look (plum night, gold lettering, pill buttons, gold dust) applied to the Diaries pages, Lounge, Readiness Book, Flight 777, Author and the books shop. Delete the two link lines in a page to return it to its old look.
