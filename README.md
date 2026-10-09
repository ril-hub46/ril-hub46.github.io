# My portfolio (Hugo)

Personal site skeleton for a Data Engineer / Data Scientist, with no external theme:
all the HTML/CSS is included, you can edit everything directly.

## Structure

- `hugo.toml` - general config (title, email, social links, CV)
- `content/_index.md` - homepage text (name, role, tagline)
- `data/skills.yaml` - your skills (2 columns: engineering / science)
- `data/experience.yaml` - your professional background
- `data/projects.yaml` - your projects (3 sample entries to replace)
- `layouts/` - HTML templates (adjust if you want to change the structure)
- `assets/css/main.css` - styling (colors, spacing, dark mode included)
- `static/cv/` - drop your CV as a PDF here, named `cv.pdf`
- `static/img/` - your images (profile photo, project screenshots...)

## Run locally

1. Install Hugo (extended): https://gohugo.io/installation/
2. From this folder:
   ```
   hugo server -D
   ```
3. Open http://localhost:1313

## Deploy to GitHub Pages

1. Create a repo named exactly `<your-username>.github.io`
2. Update `baseURL` in `hugo.toml` with the real URL
3. Build the site:
   ```
   hugo --minify
   ```
   This generates a `public/` folder.
4. Push the content of `public/` to the `main` branch (or use the
   official Hugo GitHub Action to automate the build + deployment,
   see the Hugo "Host on GitHub Pages" docs).

## Going further

- Replace the 3 sample projects in `data/projects.yaml` with your own
- Add a real photo in `static/img/`
- Adjust the colors in `assets/css/main.css` (`:root` variables)
