# DASS-21

A clean, single-file, no-tracking version of the **Depression Anxiety Stress Scales – 21 item version** (Lovibond & Lovibond, 1995). Open the page, answer 21 questions, see your three subscale scores. Everything stays in the browser — no accounts, no servers, no analytics, no cookies, no localStorage.

The whole thing is one self-contained `index.html` file (~470 lines, including styles and script). No build step. No dependencies. Works offline.

---

## Try it

If a hosted demo exists, it'll live here: `https://dass21.vercel.app` *(update this once you've deployed)*.

To run locally without any setup: download `index.html` from this repo and double-click it.

---

## Host it (pick one)

### 1. Drop the file on your existing site

Easiest possible. Download `index.html` and put it wherever you want it served. For example:

- `yoursite.com/dass21/index.html` → reachable at `yoursite.com/dass21/`
- `yoursite.com/dass21.html` → reachable at `yoursite.com/dass21.html`

It's a plain static HTML file — any web server will serve it. No build, no config.

### 2. Deploy to Vercel (one click)

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Cormacsb/dass21)

That button forks this repo into your Vercel account and gives you a live URL in about a minute. No configuration needed — Vercel auto-detects the static HTML.

### 3. GitHub Pages

Fork this repo, then go to **Settings → Pages**, set source to `main` branch / root, and click Save. Your URL will be `https://<your-username>.github.io/dass21/`.

### 4. Netlify (drag & drop)

Go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag `index.html` into the browser. You'll get a URL immediately.

### 5. Cloudflare Pages

Connect this repo (or your fork) at [pages.cloudflare.com](https://pages.cloudflare.com) — no build command, output directory is `/`.

---

## Customize it

The whole thing is one HTML file. Open it in a text editor:

- **Branding / intro text** — edit the `<h1>`, `.subtitle`, and `.instructions` block at the top.
- **Colors** — change the CSS custom properties at the top of `<style>` (`--bg`, `--accent`, etc.). Light and dark variants are both there.
- **Post-result messaging** — add anything you want after the `<div id="results">` section (e.g., links to your services, next steps, contact info).

**Do not modify the 21 question items themselves.** UNSW's licensing permits free reproduction but not modification — the validity of the scoring depends on the items being unchanged from the original instrument. If you tweak the questions, the severity bands no longer mean what they're supposed to mean.

---

## About the test

The DASS-21 is the short form of the **Depression Anxiety Stress Scales** by S.H. Lovibond & P.F. Lovibond (1995, University of New South Wales). It's a validated screening instrument widely used in clinical and research settings.

It produces three scores (Depression, Anxiety, Stress) on a 0–42 scale, each mapped to one of five severity bands (Normal, Mild, Moderate, Severe, Extremely Severe). Each subscale is the sum of 7 items scored 0–3, doubled so scores are comparable with the original 42-item DASS.

**This is a screening tool, not a diagnosis.** It can't diagnose anything — it indicates how strongly someone has experienced certain symptoms over the past week, relative to a general population. Anyone with concerning results should be encouraged to talk to a clinician.

The DASS is in the public domain. From the official UNSW page:

> "The DASS questionnaire forms may be downloaded and copied without restriction."

Canonical reference: [www2.psy.unsw.edu.au/dass](http://www2.psy.unsw.edu.au/dass/)

Citation: Lovibond, S.H. & Lovibond, P.F. (1995). *Manual for the Depression Anxiety Stress Scales* (2nd ed.). Sydney: Psychology Foundation of Australia.

---

## License

The wrapper code (HTML, CSS, JS in `index.html`) is **MIT licensed** — see [LICENSE](LICENSE). Use, modify, and redistribute freely.

The DASS-21 instrument itself (the 21 question items, scoring procedure, and severity bands) is in the public domain per UNSW. Items must be reproduced unchanged. Commercial sale of the instrument is not permitted by UNSW; non-commercial use is unrestricted.
