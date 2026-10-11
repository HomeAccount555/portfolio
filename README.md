# Henry Liang: Portfolio site

Plain HTML + CSS. No build step and no framework. To preview, run `python3 -m http.server 8000` in this folder and open http://localhost:8000. Double-clicking `index.html` also works, but the YouTube video shows "Error 153" that way. It plays fine over http and on the live site.

Built for **Co-op 101, Assignment: Portfolio Submission**. Due **Oct 11, 23:59**; submissions close Oct 18.
Graded complete/incomplete. You can resubmit as many times as you want.

## Files

```
index.html                                  Home: name, focus, one-line pitch, "See my work" button, 2 project cards
about.html                                  About + Contact (#contact)
projects/restaurant-management-system.html  Case study 1 (embeds the YouTube demo)
projects/citation-guide.html                Case study 2 (quotations poster)
style.css                                   All styling. Change colours at the top (:root)
assets/                                     Put images and the resume PDF here (currently EMPTY)
check.py                                    Pre-publish check
```

## Before you publish: run the check

```
python3 check.py
```

It must print `READY` (exit code 0). While it prints `NOT READY`, it lists every problem:
missing images, draft markers, and `REPLACE-ME` placeholders.
**The assignment fails any site with placeholder content or blank pages**, so don't submit until it says READY.

Draft text appears with a **yellow highlight** in the browser (`class="todo"`). Replace each piece with your own words,
then delete the `class="todo"` from that tag.

## What you need to provide

| # | What | Goes to | Notes |
|---|------|---------|-------|
| 1 | Quotations poster as an image | `assets/quotation-poster.jpg` | Export from Canva as PNG, or send the PDF and we'll convert it |
| 2 | Close-up crop of the poster | `assets/quotation-poster-detail.jpg` | The "How to Use Quotations" part |
| 3 | All 5 posters side by side | `assets/citation-series.png` | **Ask teammates first** and credit them by name. If they say no, delete that figure (you still need 3 images, so add another one of your own) |
| 4 | ER diagram of the restaurant database | `assets/rms-er-diagram.png` | Redraw it if needed (draw.io / Figma) |
| 5 | Two screenshots of the restaurant app | `assets/rms-screen-1.png`, `rms-screen-2.png` | You can take stills from your demo video |
| 6 | A photo of yourself | `assets/henry.jpg` | Square works best |
| 7 | Resume PDF | `assets/Henry-Liang-Resume.pdf` | **Remove your phone number and home city first.** This is a public site |
| 8 | Email + LinkedIn URL | replace every `REPLACE-ME` | Decide whether to show your email publicly |
| 9 | Challenges, outcome, reflection for both projects | yellow boxes on the project pages | The assignment requires reflection: what you learned and what you'd do differently. Write it yourself, first person |

Also check: the GitHub repo `dagemd/354-Project` is **private**, so it's not linked. If the team makes it public, you can add a link on the restaurant page.

## Publish (pick one)

**GitHub Pages (free, recommended)**
1. Create a GitHub account, then a new **public** repository, e.g. `portfolio`.
2. Upload every file in this folder (keep the `projects/` and `assets/` folders).
3. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)` → Save.
4. After a minute the site is at `https://<your-username>.github.io/portfolio/`.

**SFU personal web space** (not verified): SFU may offer students a `sfu.ca/~<computing-id>` page. Check with SFU IT Services before counting on it.

Then open the live URL in a private window (to confirm there's no password or login), click every link, and submit
the URL on Canvas. Figma links are not accepted.
