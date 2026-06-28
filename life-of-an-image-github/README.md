# The Life of an Image

A single-page forensic case file tracing how one photographic gesture — a match
frame shot straight off a living-room television — spread from a personal quirk
into an industry-wide reflex within days.

## Run it

It's a static site. Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server
# then visit http://localhost:8000
```

## Deploy on GitHub Pages

1. Push this folder to a repository.
2. Repo **Settings → Pages**.
3. Set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Your site goes live at `https://<username>.github.io/<repo>/`.

## Structure

```
index.html      the page
images/         the 9 screenshots it references (relative paths)
```

Keep `images/` next to `index.html` — the page loads photos via relative paths,
so they break if the folder is moved or renamed.
