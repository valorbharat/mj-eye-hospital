# M. & J. Institute of Ophthalmology — website

A single-page website for M. & J. Institute of Ophthalmology, Ahmedabad, styled after
the government-institutional format of the Civil Hospital Ahmedabad website, and
structured as a GitHub Pages project (same pattern as the VALOR site: one `index.html`
plus a `Webfoto` folder for images).

## Structure

```
mj-eye-hospital/
├── index.html      # the entire site (HTML + CSS in one file)
├── Webfoto/         # put all real photos here (building, OPD, doctors, camps, etc.)
└── README.md
```

## What still needs real content

Search everywhere for these placeholders and replace them before going live:

- OPD registration timings (currently marked "to be confirmed")
- Institute phone number and email address
- Director's photograph (`Webfoto/director.jpg` or similar, then update the
  `.lead-photo` block in `index.html`)
- Notice board entries (dates + real circulars/tenders)
- Gallery photos (drop files into `Webfoto/`, then swap each `<figure>` placeholder
  for an `<img src="Webfoto/your-photo.jpg">`)

Facts already filled in (establishment year, Western Regional Institute status,
director's name, department list, PG programme) come from public sources
(B. J. Medical College's website and Civil Hospital Ahmedabad) — double-check them
against the institute's own records before publishing.

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `mj-eye-hospital`).
2. Push these files to the `main` branch:
   ```
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/mj-eye-hospital.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, set the source branch to `main` and the
   folder to `/ (root)`.
4. The site will be published at:
   `https://<your-username>.github.io/mj-eye-hospital/`

No build step or server is required — it's a static HTML/CSS file, same as the
VALOR site.
