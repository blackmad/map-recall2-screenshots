# Map Recall screenshots

Screenshots that the Canal Recall **What's New** page links to
(`public/canal-drive/whats-new-notes.json` in
[blackmad/map-recall2](https://github.com/blackmad/map-recall2)). They live
here so the game repository does not grow with every release note.

## Layout

```
whats-new/YYYY-MM-DD-<note-slug>.jpg          one picture
whats-new/YYYY-MM-DD-<note-slug>-before.jpg   before/after pair
whats-new/YYYY-MM-DD-<note-slug>-after.jpg
```

- `YYYY-MM-DD` is the note's `date` (the day it reached main); the slug is the
  note title in kebab-case, shortened.
- JPEG or WebP, long edge 1600 px or less, under 400 KB each. Phone frames are
  fine at their native width.
- Never rewrite or delete a published file: the game links to it by path.
  Add a new file instead.

## Referencing from a note

```json
{
  "date": "2026-10-30",
  "title": "Ride off from a standstill on squares",
  "text": "...",
  "images": [
    { "src": "whats-new/2026-10-30-squares-before.jpg", "alt": "Bike stuck on the Nieuwmarkt", "caption": "Before" },
    { "src": "whats-new/2026-10-30-squares-after.jpg",  "alt": "Bike riding off the Nieuwmarkt", "caption": "After" }
  ]
}
```

`src` is a path in this repository; the page prefixes
`https://raw.githubusercontent.com/blackmad/map-recall2-screenshots/main/`.
A full `https://` URL is also accepted.

## Adding

```sh
cp shot.jpg whats-new/2026-10-30-squares-after.jpg
git add whats-new && git commit -m "whats-new: squares after" && git push
```

## Review strips

```
review/YYYY-MM-DD-<lane-slug>-<what>.jpg
```

Before/after strips a lane produced for a decision that is still open (a
flag flip, a kit batch). They are larger than What's New images (native
width, under 2 MB) and are linked from the `needs-david` issue that asks the
question. Once decided, the What's New note gets its own `whats-new/` copy.
