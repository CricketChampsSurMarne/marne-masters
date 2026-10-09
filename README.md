# Marne Masters Club de Cricket website

Files:
- `index.html` — the website
- `events.js` — the upcoming events list (the only file you need to edit regularly)
- `logo.png` — the club logo
- `favicon.png` — the small logo shown in the browser tab

## 1. Put the site online for free (GitHub Pages)

1. Create a free account at https://github.com
2. Click **New repository**, name it e.g. `marne-masters`, set it to **Public**, click **Create**.
3. Click **uploading an existing file**, drag in all the files from the folder (`index.html`, `events.js`, `logo.png`, `favicon.png`, `README.md`), then **Commit changes**.
4. Go to **Settings > Pages**. Under "Branch", choose `main` and `/ (root)`, click **Save**.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/marne-masters/`

(Alternative: drag the folder onto https://app.netlify.com/drop — but then you must re-upload the folder each time you change events.)

## 2. Activate the contact form (one time only)

The form sends emails to cricketchampssurmarne@gmail.com through the free service FormSubmit.
The **first** time someone sends a message from the live site, FormSubmit sends an activation email
to that Gmail address. Open it and click **Activate Form**. After that, every message arrives as a normal email
(check the spam folder the first time). Hitting "Reply" answers the sender directly.

## 3. Edit upcoming events

On GitHub, open `events.js`, click the pencil icon, edit, then **Commit changes**. The site updates in about a minute.

Each event looks like this:

```js
{
  date: "2026-10-17",
  time: "10:00 - 12:00",
  title: "Séance d'initiation",
  title_en: "Beginner session",
  place: "Gymnase Pablo Picasso",
  details: "Découvrez le cricket avec nos entraîneurs.",
  details_en: "Discover cricket with our coaches.",
  tag: "Initiation",
  tag_en: "Beginners"
},
```

Each event has French fields (`title`, `place`, `details`, `tag`) and optional English
versions (`title_en`, `place_en`, `details_en`, `tag_en`). If an English field is missing, the French text is shown.
Keep the quotes and the comma between events. Past events disappear automatically; if there are none,
the site invites visitors to join the WhatsApp group.

## 4. Other notes

- The "Where we play" section automatically opens on the indoor venue from September to May and the outdoor ground from June to August.
- The site opens in French. Visitors can switch with the EN - FR toggle in the menu, and their choice is remembered on their device. To change the outdoor ground's name (currently "Terrain extérieur"), search `out_name` in `index.html`.
