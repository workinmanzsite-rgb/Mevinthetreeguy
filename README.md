# Melvin the Tree Guy — Website

The official homepage for **Melvin the Tree Guy**, a locally owned tree service.
This is a single-file static website (`index.html`) — no build step, no
dependencies, no frameworks. Upload it to GitHub Pages (or any static host) and
it's live.

---

## 🌳 About the Business

Melvin the Tree Guy provides professional tree care and land clearing, including:

- Tree trimming & pruning
- Tree removal
- Logging
- Brush removal
- Stump grinding
- Firewood
- Storm damage cleanup & removal

**Free estimates on every job.**

| | |
|---|---|
| **Phone** | (417) 969-8066 |
| **Facebook / Messenger** | https://www.facebook.com/profile.php?id=61593145693724 |
| **Estimates** | Free |

---

## 🖥️ What's on the Page

The homepage is a one-page site with these sections, top to bottom:

1. **Free estimates banner** — always visible at the very top
2. **Sticky header** — business name, "Call Now" button, "Messenger" button
3. **Hero** — headline, short intro, and two big action buttons
   (Call / Message on Facebook)
4. **Services** — 7 cards covering every service offered
5. **Why Melvin** — trust points (free estimates, locally owned, clean job
   sites, storm-ready)
6. **Contact** — a centered card with large Call and Messenger buttons plus
   the phone and Facebook details
7. **Footer** — business summary, contact links, service list, copyright

The page is **mobile-first** — designed to be opened and used from a phone,
which is how most customers will find it.

---

## 🚀 How to Deploy (Phone Only, No Computer)

1. Open [github.com](https://github.com) in your phone browser and sign in.
2. Tap **+ → New repository**.
   - Name it something like `melvin-tree-guy`
   - Set visibility to **Public** (required for free GitHub Pages)
   - Check **Add a README file**
   - Tap **Create repository**
3. Tap **Add file → Create new file**.
   - Name the file exactly **`index.html`**
   - Paste the full HTML
   - Tap **Commit new file**
4. Tap **Settings → Pages**.
   - Under "Branch," select **`main`**
   - Keep the folder as **`/ (root)`**
   - Tap **Save**
5. Wait 1–2 minutes, refresh the Pages settings screen, and the live URL will
   appear (usually `https://yourusername.github.io/melvin-tree-guy/`).

That URL is the site. Share it on Facebook, put it in a text, or print it on a
business card.

---

## ✏️ What to Update Later

Everything is in `index.html`. Search for these strings to find and edit them:

| Search for | What it is |
|---|---|
| `(417) 969-8066` | Phone number (appears in several places) |
| `tel:+14179698066` | Tap-to-call link (keep the `+1` and no spaces) |
| `61593145693724` | Facebook profile ID — appears **4 times** |
| `Melvin the Tree Guy` | Business name |

### If Melvin gets a Facebook username

Right now the link points to his profile ID. If he claims a username later
(e.g. `facebook.com/melvinthetreeguy`), search the HTML for
`61593145693724` and replace the whole URL in all 4 places. The buttons will
then go to the cleaner link.

### Adding photos

The page currently uses an inline SVG tree graphic, so no image files are
needed. To add real job photos:
1. Upload images to the repo (Add file → Upload files).
2. Add `<img src="yourphoto.jpg" alt="...">` tags in the service cards or a new
   gallery section.

### Adding hours or a service area

Not listed yet. If Melvin wants them shown, add a line inside the contact card
(`<div class="contact-detail">`) or the footer.

---

## 🎨 Changing Colors

All colors are defined in one place at the top of the CSS:

```css
:root{
  --green:#1f6b3a;       /* main brand color */
  --green-dark:#134d29;  /* headings, banner, hover */
  --green-light:#e8f3ec; /* soft backgrounds */
  --bark:#3b2f2a;        /* footer */
  --cream:#faf8f4;       /* page background */
  --fb:#1877f2;          /* Facebook blue */
}
