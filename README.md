# Reality is Buffering Comic
**BY:G33KY**

Comic reader site hosted via GitHub Pages.

---

## Folder Structure

```
/
├── index.html          ← main comic reader page
├── images/
│   ├── banner.png                        ← hero banner at top of site
│   ├── character-lore/
│   │   ├── cover.jpg
│   │   ├── page1.jpg
│   │   ├── page2.jpg
│   │   └── ...
│   ├── issue1-dragonform/
│   │   ├── cover.jpg
│   │   ├── page1.jpg
│   │   └── ...
│   ├── issue2-ghostmode/
│   │   ├── cover.jpg
│   │   ├── page1.jpg
│   │   └── ...
│   └── issue3-latenightshenanigans/
│       ├── cover.jpg
│       ├── page1.jpg
│       └── ...
└── README.md
```

---

## How to Add a New Page

1. Upload the image file to the correct issue folder under `/images/`
2. Open `index.html`
3. Find the `COMIC_DATA` object near the bottom of the file (inside the `<script>` tag)
4. Add the filename to the `pages` array for that issue:

```js
'issue1': {
  folder: 'images/issue1-dragonform',
  pages: [
    'page1.jpg',
    'page2.jpg',
    'page3.jpg',
    'page4.jpg',  // ← add new page here
  ]
}
```

5. Commit the changes — the site updates automatically.

---

## How to Add a New Issue

1. Create a new folder under `/images/` (e.g. `issue4-newissuename/`)
2. Upload your cover and pages to it
3. In `index.html`, add a new tab button and panel following the existing pattern
4. Add an entry to `COMIC_DATA`

---

## Live Site
`https://ad0rkableg33k.github.io/realityisbuffering`
