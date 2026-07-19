# Biblical Language Drill — Hebrew & Greek

I built this because I wanted a simple way to brush up on my Hebrew and Greek after letting those skills get rusty for a few years. It's a browser-based recognition drill for rebuilding Biblical Hebrew vowel points and the Greek alphabet. Pick a language, complete a timed 60-item session, and see how you did.

No login, no tracking, no ads. It runs entirely in your browser and works on desktop or mobile.

## What it does

- **Two drills, one interface.** Choose Hebrew (vowel points) or Greek (alphabet) from the landing page. Each runs as its own 60-item session.
- **Timed.** Every answer is timed. At the end of each session you'll see your accuracy, average response time, and the three characters that slowed you down the most.
- **Session-only.** Nothing is saved or synced. Every session starts fresh. I chose not to keep persistent scores because the goal is improving recognition, not chasing numbers.

## The target

Aim for 90%+ accuracy while averaging under two seconds per item.

If you're accurate but slow, you're still thinking through the answer instead of recognizing it automatically. Fast recognition is what eventually makes reading feel natural.

## One limitation

This drills recognition, not reading.

Recognizing a character is only the first step. The real skill is reading unfamiliar pointed or accented words out loud, and no multiple-choice drill can teach that. Use this to rebuild recognition speed, then spend time reading actual biblical texts.

It's also not a course. Pair it with a real grammar — Pratico and Van Pelt for Hebrew, Mounce for Greek — and use this for the drilling those books can't do for you.

## Files

```text
index.html             The application
SBL_BLit.ttf           SBL BibLit font
SBL_Font_License.txt   Copy of the SBL Font EULA
```

## Fonts and licensing

Hebrew and Greek are displayed using SBL BibLit, a widely used font in biblical studies from the Society of Biblical Literature (Tiro Typeworks).

The SBL Font EULA permits embedding the font in non-commercial electronic documents, including web pages, provided the font is unmodified and a copy of the license accompanies it. This repository includes the required license file. I do not own this font.

- Font: https://www.sbl-site.org/educational-resources/biblical-fonts/
- License: `SBL_Font_License.txt`

Note: The `@font-face` rule in `index.html` expects the font file to be named `SBL_BLit.ttf` and located in the same directory. GitHub Pages is case-sensitive, so if the filename doesn't match exactly, Hebrew and Greek will fall back to a system font.

## Hosting on GitHub Pages

1. Place `index.html`, `SBL_BLit.ttf`, and `SBL_Font_License.txt` in the repository root.
2. Go to Settings → Pages.
3. Deploy from the `main` branch using the root folder.
4. After a minute or two, your site should be available at:

```text
https://<username>.github.io/<repo>/
```

If the Hebrew or Greek doesn't render correctly, the first thing to check is that the font filename matches exactly.

## Notes

- Number keys 1–4 select an answer.
- Enter or Space advances to the next item.
- Hebrew and Greek are intentionally kept in separate sessions. Mixing scripts seemed to slow recognition when I tested it, so switching languages starts a new session instead.
