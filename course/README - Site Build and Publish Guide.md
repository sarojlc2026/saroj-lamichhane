# The Site — What Is Built and How to Publish It

**15 pages · 4 embedded video modules · 41 downloadable course files · 0 accessibility failures · 0 broken links**

Open `index.html` in a browser to see it.

---

## The course now uses your real materials

The four video modules from `Resources/Digital Training Accessibility Course` are embedded, with your actual transcripts, quick guides, apply-it activities and knowledge checks attached to each.

| Module | Topic | Video | Chapters | Downloads |
|---|---|---|---|---|
| 1 | Accessibility Overview | 13 MB | 6 | 5 |
| 2 | Accessible Microsoft Word Documents | 26 MB | 10 | 8 |
| 3 | Accessible Microsoft PowerPoint Documents | 35 MB | — | 7 |
| 4 | Accessible PDF Documents | 15 MB | 7 | 13 |

**Chapter markers** were generated from the timestamps in your transcripts, so viewers can jump to "Operable design" or "Document Title and Language" directly. Module 3's transcript is a Camtasia export with no timestamps, so it has no chapter track — everything else about that module is identical.

**Every transcript is on the page** in an expandable panel, with stage directions and timestamps styled distinctly, plus a download link to the original `.txt`.

The five written modules I drafted earlier are kept as **companion guides** — alternative text, captions, LMS structure, auditing, and AI in assignment design. They are clearly labelled as written guides so nothing implies they are part of your recorded course.

---

## ⚠️ Check before publishing: are your videos captioned?

I embedded the MP4 files as supplied. **I cannot verify from the files whether captions are burned in or embedded.** You teach this in Module 1, and it is the first thing a knowledgeable viewer will check.

- **If captions are burned into the video**, you are fine.
- **If not**, export a `.vtt` caption file for each and add one line to each module page, immediately after the `<source>` line:

```html
<track kind="captions" src="media/module-1.vtt" srclang="en" label="English" default>
```

The transcripts you already have make producing the `.vtt` files quick, and most caption editors will export directly.

---

## ⚠️ Institutional ownership

These materials carry TIDE and Texas A&M University-Texarkana branding, and were produced as part of your employment. **Confirm in writing that you may publish them openly before you do.**

The footer currently credits: *"Course materials © Saroj Lamichhane, produced with Technology Innovation and Digital Education (TIDE), Texas A&M University-Texarkana. Shared under CC BY 4.0."* Adjust to whatever your institution agrees to.

If permission is delayed, publish the companion guides and the course structure, and mark the videos "available on request."

---

## Before publishing: replace the placeholders

| Placeholder | Replace with | Count |
|---|---|---|
| `REPLACE_EMAIL` | your email address | ~34 |
| `REPLACE_GITHUB` | your GitHub repository URL | ~17 |
| `REPLACE_LINKEDIN` | your LinkedIn URL | ~16 |
| `REPLACE_FILE_SLIDES` | OLC Innovate slides | 1 |

Find-and-replace across the folder.

---

## Hosting: the videos change the calculation

The site is **115 MB**, of which 90 MB is video.

**Recommended — host video externally, site on GitHub Pages.** Upload the four MP4s to YouTube (unlisted or public) or Vimeo, then replace each `<video>` block with the platform's embed. Site drops to ~25 MB, videos stream properly, and the platform handles caption display. Your viewers get a better experience.

**Alternative — everything on GitHub Pages.** Works. 115 MB is within limits, but a soft 1 GB repository recommendation applies and the initial push is slow. Fine if you prefer everything in one place.

**Alternative — Netlify Drop.** Drag the `site` folder to app.netlify.com/drop. Live in two minutes, handles video adequately.

---

## Accessibility, verified programmatically

Across all 15 pages: exactly one `<h1>` each, no skipped heading levels, `lang="en"`, `<!DOCTYPE html>`, semantic landmarks, skip-to-content link, `aria-current` on active navigation, breadcrumb and pager navigation labelled, no images without alt text, no vague link text, real `<table>` markup with `<th scope="col">` and captions, transcripts in natively keyboard-accessible `<details>`, visible focus indicators, contrast above 4.5:1, `prefers-reduced-motion` respected, print stylesheet.

**Video specifically:** native `<video controls>` with keyboard-operable controls, `preload="metadata"` so pages load fast, a text fallback with a download link for browsers that cannot play it, and chapter tracks where source timestamps allowed.

Run WAVE (wave.webaim.org) once live to confirm end to end, and test one video page with a screen reader.

---

## What this does for the petition

Your Statement of Intent, Phase 1, commits to publicly releasing this documentation under an open licence. **This is that**, dated and verifiable the moment you publish.

It also answers a question an officer could otherwise ask. Your petition says Dr. Vance and Dr. Paudel found and used publicly available materials. From publication onward there is a permanent, findable address where those materials live.

Capture a dated PDF of the site once live — it may be worth a late exhibit.
