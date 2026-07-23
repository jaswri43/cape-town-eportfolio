# Cape Town ePortfolio

Three pages: `index.html` (Overview + Thank You), `reflections.html` (Reflection
Summary + all 6 weekly lessons), `project.html` (MERLS walkthrough).

## Adding your photos

Drop image files into the matching folder under `assets/img/`:

- `assets/img/hero/` — your Table Mountain / GRIT workspace photo
- `assets/img/thankyou/` — group photo with GRIT / EDU Africa
- `assets/img/weeks/` — one or two photos per week
- `assets/img/walkthrough/` — MERLS screenshots

Then in the HTML, find the matching `<div class="photo-slot">...</div>` block
and replace it with an `<img>` tag, e.g.:

```html
<!-- before -->
<div class="photo-slot wide">[ HERO PHOTO — ... ]</div>

<!-- after -->
<div class="photo-slot wide">
  <img src="assets/img/hero/table-mountain.jpg" alt="View from Table Mountain">
</div>
```

The dashed border disappears automatically once a real `<img>` is inside —
the CSS just fills the frame.

## Editing text

Everything is plain HTML — open any `.html` file and edit the text directly
between the tags. No build step, no dependencies.

## Deploying with GitHub Pages

1. Create a new repository on GitHub (public).
2. Upload all these files (drag-and-drop works in the GitHub web UI, or `git push`).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch",
   branch `main`, folder `/ (root)`. Save.
5. Wait a minute or two — GitHub will give you a live link like
   `https://yourusername.github.io/repo-name/`.
