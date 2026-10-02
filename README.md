# HEBREW HACK · Your Hebrew Journey

Draft course-journey map for KNIZ. Embed it on a Systeme.io lesson with a custom HTML block:

```html
<iframe src="https://yagelkniz.github.io/HEBREW-HACK--MAP/?station=6" style="width:100%;aspect-ratio:16/9;border:0;" loading="lazy"></iframe>
```

Change `6` to the station the student is on. Stations before that number are completed, that station shows the “you are here” pin, and the rest stay locked. A number past the last station marks the whole road complete. Leave off `?station` for the base map, with nothing completed:

```html
<iframe src="https://yagelkniz.github.io/HEBREW-HACK--MAP/" style="width:100%;aspect-ratio:16/9;border:0;" loading="lazy"></iframe>
```

The map is drawn at 1920×1080 and scales to the iframe, keeping 16:9, so the iframe itself should stay 16:9 (the `aspect-ratio` above does that). There is no scrollbar inside the frame.

## Edit the stations

Open `index.html` and edit the `STATIONS` list at the top of the script. Each station has:

- `tag` — small coral label, shown in capitals (`Step 1` becomes STEP 1)
- `label` — English name
- `hebrew` — Hebrew with its niqud, or `""`
- `hebrewAlt` — optional second Hebrew word, drawn blue / pink (Gender uses this)
- `subtitle` — muted English line, or `""`
- `icon` — an emoji, or `ALEF`, `SEGOL`, or `GENDER`
- `link` — lesson URL. Leave `""` and the station is not clickable. A link opens with `target="_top"` so the lesson replaces the Systeme.io page instead of loading inside the frame.

About 8–14 stations works best. The road reflows when you add or remove one. Push to `main` and GitHub Pages updates the embed.
