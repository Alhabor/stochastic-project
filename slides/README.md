# Presentation Slides

A self-contained HTML slide deck (19 slides, ~20 minutes including the live
demo). No build step, no dependencies — `index.html` plus the figure PNGs in
`assets/`.

## Present locally

```bash
python3 slides/present.py
```

This serves the deck at http://localhost:8700 and opens it in your browser.
The demo slide's **"Open the dashboard"** button always opens the public
Streamlit deployment, so the presentation does not depend on the presenter's
computer running Python.

Alternatively, open `slides/index.html` directly or serve it with any static
server. The public dashboard link works in either case.

Controls: **←/→** (or space / click) to navigate · **N** toggles speaker
notes · **Home/End** jump · URL hash (`#/12`) deep-links a slide · print to
PDF via the browser for a handout.

## Speaker script

`Speaker_Script.docx` is a verbatim presenter script — one section per slide
with timing marks (~20 minutes total), stage directions in italics, a
pre-talk setup checklist, the 5-step demo walkthrough, and prepared answers
for likely questions. Regenerate it with:

```bash
npm install docx && node slides/build_speaker_script.js
```

## The live-demo slide

Slide 18 opens the public dashboard at
https://alhabor-stochastic-project.streamlit.app/. No software or local server
is required on the presentation computer.

Tip: open the dashboard once ~a minute before the demo so a sleeping Community
Cloud app can wake up off-stage. Bundled sample markets avoid dependence on the
live Polymarket API, but the professor's computer still needs internet access.

## Web deployments

- Slides: https://show.alhabor.com/2026/stochastic-project/
- Dashboard: https://alhabor-stochastic-project.streamlit.app/
