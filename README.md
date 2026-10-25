# Living the Best Version of You

A short, anonymous handbook for being yourself.

Think of a radio, not a railway. A railway says there is one track and you ride it
to the end. A radio says every station is playing right now — you only hear the one
you are tuned to.

Four laws, one belief worth digging up, a compass, and pocket cards for a hard day.
Takes about ten minutes.

---

## What it is

A single self-contained HTML page. No build step, no framework, no dependencies,
no server. Open `index.html` in any browser and it works — from a web host, a USB
stick, or a folder on a school laptop with the wifi off.

**Nothing is saved and nothing is sent.** There is no account, no analytics, no
cookies, no local storage, and no network requests of any kind. Whatever a reader
types stays in their browser tab and disappears when they close it. The only outbound
link on the page is [findahelpline.com](https://findahelpline.com), and only if
someone chooses to click it.

The fonts are embedded directly in the file, so the page does not phone home to
Google or anyone else. This matters if it ends up in a school.

## How it works

- **Five doors** — Young at Heart, Wild Free Heart, Restless Heart, Weathered Heart,
  Long Way Round. The four laws are the same for everyone; the examples change.
- **A mood check** — sets the tone of the writing and dims the lamp behind the page.
  Choosing "Hurting" routes to a gentler branch with helpline information first.
- **Say it simpler** — a toggle in the footer, live on every screen. The page opens
  in the simpler register by default; the fuller one is one tap away.
- **Everything is skippable.** The belief excavation has an exit on every step.

## Publishing it

### GitHub Pages

1. Create a new **public** repository.
2. Upload `index.html`, `README.md`, `LICENSE`, `FONT-LICENSES.txt` and `.nojekyll`.
3. Go to **Settings → Pages**.
4. Under *Build and deployment*, set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`. Save.
5. Wait a minute or two. Your page appears at
   `https://<your-username>.github.io/<repo-name>/`

The `.nojekyll` file tells GitHub not to run the files through Jekyll. Nothing here
needs it, and it makes the deploy faster and less surprising.

### Anywhere else

Drag `index.html` onto [Netlify Drop](https://app.netlify.com/drop) for an instant
URL, or drop it on any web host. It is one file. It has no opinions about where it lives.

## Changing the words

All the copy lives in plain JavaScript objects near the top of the `<script>` block,
so you can edit the text without touching the layout:

| Object | What it holds |
| --- | --- |
| `COPY` | Every fixed line on every screen |
| `LAWS` | The four laws, with a passage per door |
| `DIG` | The six excavation steps |
| `POCKET` | The printable pocket cards |
| `DOORS`, `MOODS` | The two opening questions |

Most entries are a `{rich, plain}` pair — the fuller wording and the simpler one.
If you add a door to `DOORS`, give every law in `LAWS` a matching key or that door
will render blank.

## Licence

The writing is released under **CC BY-NC-SA 4.0** — copy it, translate it, adapt it,
put it in front of whoever needs it, as long as you credit it, don't sell it, and
share what you make under the same terms. See `LICENSE`.

The embedded fonts — Bodoni Moda, Newsreader and IBM Plex Mono — are licensed
separately under the SIL Open Font License 1.1. See `FONT-LICENSES.txt`.

## A note on what this is not

This is a page. It is decent company and a poor substitute for a person.

If you are sharing it with young people, share the helpline alongside it.
[findahelpline.com](https://findahelpline.com) lists crisis lines by country.
Nothing on the page matters more than that.
