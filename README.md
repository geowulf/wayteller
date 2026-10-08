# The Wayteller — website

Static site for the Wayteller brand, hosted free on GitHub Pages.

## Structure

| Page | Path | Notes |
|---|---|---|
| Home | `/` | Brand statement, vote banner, cards |
| About | `/about/` | About Greg |
| Blog | `/blog/` | Story listing (add posts as `/blog/slug/index.html`) |
| Podcast | `/podcast/` | Episode listing |
| Book | `/book/` | Rideshare Confessions (in progress) |
| Vote | `/vote/` | **Temporary** — Top Host 2026 vote page, retires when voting ends (Dec 2026) |

## Publishing a new blog post

1. Copy `blog/index.html`'s structure into `blog/my-story-title/index.html`.
2. Add a link to it in `blog/index.html`.
3. Commit and push — GitHub Pages redeploys automatically.

## Retiring the vote page

After the contest ends: delete the `/vote/` folder, remove the vote banner
from `index.html`, and remove Vote from the nav in every page. The QR code
asset lives at `assets/vote-qr.png`.

## Local preview

```sh
cd wayteller-site
python3 -m http.server 8000
# open http://localhost:8000
```
