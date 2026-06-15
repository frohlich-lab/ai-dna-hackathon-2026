# AI × DNA Hackathon 2026

Static GitHub Pages site for the AI × DNA Hackathon at the Francis Crick Institute, 6–7 July 2026.

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `ai-dna-hackathon-2026`)
2. Push this directory:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add hackathon site"
   git branch -M main
   git remote add origin https://github.com/<your-org>/<repo>.git
   git push -u origin main
   ```
3. Go to **Settings → Pages → Source**: select **Deploy from branch**, branch `main`, folder `/ (root)`
4. Site goes live at `https://<your-org>.github.io/<repo>/`

## Preview locally

Open `index.html` directly in a browser (no server needed), or:

```bash
python3 -m http.server 3456
# → http://localhost:3456
```

## Customisation

All content is in `index.html`. Key areas to update:

| What | Where |
|------|-------|
| Speaker details | `#speakers` section |
| Schedule times | `#schedule` section, `data-type` attributes control colour |
| Track descriptions | `#tracks` section |
| Venue address | `#venue` section |
| Organiser names | `#organisers` section |
| Colour palette | `:root` CSS variables at the top of `<style>` |
