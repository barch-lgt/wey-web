# weyai.com.et

Static site served by GitHub Pages (`index.html` + `CNAME`).

## Adding real photos / videos
Every visual in the page is a "media slot" (`<div class="slot">`) that currently shows a generated animation.
Add an attribute to swap in real media — nothing else to change:

| Want | Add to the `.slot` div |
|------|------------------------|
| Photo | `data-img="media/team.jpg"` |
| Looping video | `data-video="media/loop.mp4"` (optional `data-poster="media/poster.jpg"`) |
| YouTube / Vimeo | `data-embed="https://www.youtube.com/embed/VIDEO_ID"` |
| Showreel modal (Wey Call section, `#reelSlot`) | `data-video="media/showreel.mp4"` or `data-embed="..."` |

Put files in a `media/` folder in this repo. If a file fails to load, the generated visual stays.

## Languages
EN / አማ / OM / ትግ switcher lives in the `LANG` object in `index.html`. Missing keys fall back to English.
Have a native speaker review the Amharic, Afaan Oromoo and Tigrinya strings (including the demo-call dialogues in `CALLS`).
