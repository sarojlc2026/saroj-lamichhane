# The Site Is Built — How to Publish It

Five working, accessible HTML pages. Open `index.html` in a browser right now to see it.

**Verified before delivery:** one `<h1>` per page, no skipped heading levels, semantic landmarks (`header`/`nav`/`main`/`footer`), skip-to-content link, `lang="en"`, descriptive link text throughout, visible focus indicators, contrast above 4.5:1, responsive, and `prefers-reduced-motion` respected.

---

## Step 1 — Replace the placeholders (20 minutes)

Open all five files in any text editor and find-and-replace across the folder:

| Placeholder | Replace with | Count |
|---|---|---|
| `REPLACE_EMAIL` | your email address | 13 |
| `REPLACE_GITHUB` | your GitHub repository URL | 7 |
| `REPLACE_LINKEDIN` | your LinkedIn URL | 6 |
| `REPLACE_FILE_AUDIT_PDF` | link to the audit protocol PDF | 1 |
| `REPLACE_FILE_AUDIT_XLSX` | link to the logging template | 1 |
| `REPLACE_FILE_BLOOM_PDF` | link to the Bloom's-AI framework | 1 |
| `REPLACE_FILE_BLOOM_DOCX` | link to assignment templates | 1 |
| `REPLACE_FILE_STEM_ZIP` | link to the STEM pack | 1 |
| `REPLACE_FILE_TEMPLATES_ZIP` | link to the document templates | 1 |
| `REPLACE_FILE_IMSCC` | link to the Canvas export | 1 |
| `REPLACE_FILE_SYLLABUS` | link to the syllabus PDF | 1 |
| `REPLACE_VIDEO_URL` | walkthrough video URL | 1 |
| `REPLACE_FILE_SLIDES` | OLC Innovate slides | 1 |

For files, either drop them in a `files/` subfolder and link relatively (`files/audit-protocol.pdf`), or upload to Drive and paste share links. Relative paths are cleaner and keep everything in one place.

If a file is not ready, delete that list item rather than leaving a dead link.

---

## Step 2 — Publish

### Option A — GitHub Pages *(recommended, ~10 minutes, free)*

1. Create a GitHub account if you do not have one
2. New repository, name it `saroj-lamichhane` or similar, set to **Public**
3. Upload all five `.html` files and your `files/` folder
4. **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save**
5. Live in a minute or two at `https://YOURNAME.github.io/REPO/`

**Why this over Google Sites for your situation:** the repository timestamps every commit publicly. Your petition claims these are open materials others adopt independently. A repo with dated commits evidences that in a way a website cannot. It is also where practitioners expect to find open resources.

Add a custom domain later if you want (Settings → Pages → Custom domain, about $12/year).

### Option B — Google Sites

Google Sites will not accept raw HTML pages, so use these files as your source and paste content across:

1. sites.google.com → blank site
2. Create five pages matching the filenames
3. Open each HTML file in a browser, copy the visible text, paste into the matching Google Sites page
4. Rebuild headings with the **Title / Heading / Subheading** styles — do not paste and bold
5. Upload files to Drive and link them

Slower, and you lose the built-in accessibility work. Use it only if you specifically want Google Sites.

### Option C — Netlify Drop *(fastest, 2 minutes)*

Go to app.netlify.com/drop and drag the `site` folder onto the page. Live immediately at a random URL you can rename. No account needed to start.

---

## Step 3 — Test before sharing

1. **WAVE** — paste your live URL at wave.webaim.org and resolve every error
2. **Keyboard only** — tab through every page; you must reach every link and always see focus
3. **Mobile** — open on your phone; most faculty will
4. **Private window** — confirm it is actually public before sending the link

---

## Before you send it to anyone

Check every figure against your final petition: **34 courses, 136 faculty, 121 hours, 22 sections, 171 students at 81.3%, four states.** If a recommender repeats a number from the site that contradicts the filing, you have created a three-document inconsistency.

And do not add a page addressed to your recommenders. See `00 - START HERE`, first warning.
