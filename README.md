# biblangtools
# Biblical Language Drill — Hebrew & Greek

I wanted something to help me practice my Hebrew and Greek after a few years of abandoning my skills. Enter this  browser-based recognition drill for rebuilding **Biblical Hebrew vowel points** and the **Greek alphabet** to automaticity. One page, pick a language, run a timed 60-item session. Free, no login, no tracking, works on phone or desktop.

## What it does

- **Two drills, one interface.** Choose Hebrew (vowel points) or Greek (alphabet) from the landing page. Each runs as its own separate 60-item session.
- **Timed.** Every answer is timed. The end-of-session summary shows your accuracy, average seconds per item, and your three slowest characters that session — so you know exactly where the rust is.
- **Session-only.** Nothing is saved or synced. Each session starts fresh. This is deliberate: a persistent score is easy to game, and gaming the number defeats the point.

## The target

Aim for **90%+ accuracy AND under 2 seconds per item.** Accurate-but-slow means you're still *computing* each character rather than *knowing* it — and slow recognition makes real reading impossible. Chase the clock, not just the score.

## One honest limitation

This drills **recognition** — seeing a character and naming it. That's the necessary first step, but it is **not reading**. The real skill is decoding unfamiliar pointed/accented words *out loud*, which no multiple-choice tool can test. Use this to rebuild fast recognition, then get into actual text and read aloud. Don't let a high score convince you that you can read yet.

## Files

```
index.html          The drill (rename from biblical-language-drill.html)
SBL_BLit.ttf        SBL BibLit font — Hebrew, Greek, and Latin in one file
SBL_Font_License.txt Copy of the SBL Font EULA (required alongside the font)
```

## Fonts / licensing

Hebrew and Greek render in **SBL BibLit**, the academic-standard font from the Society of Biblical Literature (Tiro Typeworks). The SBL Font EULA permits embedding in non-commercial electronic documents, including web pages, provided the font is unmodified and a copy of the license accompanies it. This project is non-commercial and ships the license file alongside the font per that requirement. I DO NOT OWN THIS FONT.

- Font: https://www.sbl-site.org/educational-resources/biblical-fonts/
- License: see `SBL_Font_License.txt` in this repo

**The `@font-face` in `index.html` expects the font file to be named exactly `SBL_BLit.ttf`, in the same folder.** GitHub Pages is case-sensitive — if the filename doesn't match, the Hebrew and Greek fall back to a system font.

## Hosting on GitHub Pages

1. Put `index.html`, `SBL_BLit.ttf`, and `SBL_Font_License.txt` in the repo root.
2. Settings → Pages → deploy from `main` branch, root folder.
3. Live in ~2 minutes at `https://<username>.github.io/<repo>/`.
4. Open it on a phone and confirm the Hebrew pointing renders sharp (SBL BibLit), not a plain fallback. If it looks plain, the font filename didn't match — check step 1.

## Notes

- Keyboard: number keys **1–4** answer, **Enter** / **Space** advances to the next item.
- The two languages never mix within a session — switching is a clean mode change, not a blend. (Mixing scripts mid-drill causes interference; keeping them separate is intentional.)
