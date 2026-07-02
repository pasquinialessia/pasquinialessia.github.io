# pasquinialessia.github.io

Personal website — [pasquinialessia.github.io](https://pasquinialessia.github.io/)

Built as a single self-contained `index.html`: all CSS and JavaScript are inline,
and the fonts (Newsreader + Inter) load from Google Fonts. There is **no build step**
and **no framework** — edit the HTML, commit, and GitHub Pages redeploys automatically
(usually within a minute or two; hard-refresh with Cmd/Ctrl+Shift+R if you don't see changes).

## File structure

```
index.html                      ← the whole site (edit this)
images/
  biopic.jpg                    ← portrait shown in the About section
assets/
  CV_Alessia_Pasquini.pdf       ← linked by the CV buttons (add this file)
README.md
```

That's all the site needs. The old `assets/css`, `assets/js`, and `assets/webfonts`
folders from the previous template are no longer used and can be deleted.

## How to update the content

Everything lives in `index.html`. Open it and look for these spots:

- **Portrait** — replace `images/biopic.jpg`, or change the `src` on the `<img>` in the About section.
- **CV** — add your PDF at `assets/CV_Alessia_Pasquini.pdf`. It's linked in three places
  (nav, hero button, contact row); update the path there if you name the file differently.
- **Projects** — in the `#work` section. Each project is one `<a class="work-item">` block.
  Copy the block to add more, delete blocks to remove. Lead each with a **result** (a number
  if you have one), then one line of context, then the tech tags, then the link.
- **Toolkit** — the keyword chips in the About section (`.tk-row`). Keep only what's true.
- **Experience** — the timeline in `#experience`. Each entry is one `.t-item` block.
- **Text/links** — bio, contact email, and social links are plain HTML; edit in place.

Placeholders still to fill are marked with `[square brackets]` and `<!-- TODO -->` comments.

## Notes

- The site is responsive, keyboard-accessible, and respects reduced-motion preferences.
- Keep the `.git` folder and any `CNAME` file (custom domain) — don't delete those.
