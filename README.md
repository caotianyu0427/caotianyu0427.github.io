# Tianyu Cao (曹天雨) — Academic Homepage

Personal academic website for **Tianyu Cao (曹天雨)**, Postdoctoral Fellow at Johns Hopkins School of Medicine.

Built with [Hugo](https://gohugo.io/) and the [HugoBlox Academic CV](https://github.com/HugoBlox/theme-academic-cv) theme. Features English/Chinese bilingual support.

## Live Site

[caotianyu0427.github.io](https://caotianyu0427.github.io)

## Local Development

```bash
# Install Hugo (macOS)
brew install hugo

# Clone this repo
git clone https://github.com/caotianyu0427/caotianyu0427.github.io.git
cd caotianyu0427.github.io

# Install dependencies
npm install

# Start local server
hugo server
```

Open [http://localhost:1313](http://localhost:1313) in your browser.

## How to Update Content

### Update your bio / personal info
Edit `data/authors/me.yaml` — change `bio`, `role`, `affiliations`, `education`, `experience`, `awards`, etc.

### Update the English main page
Edit `content/en/_index.md` — modify the research description, contact info, or add/remove sections.

### Update the Chinese main page
Edit `content/zh/_index.md` — modify the Chinese version of all content sections.

### Add a new publication
1. Create a new folder under both `content/en/publications/your-paper-slug/` and `content/zh/publications/your-paper-slug/`
2. Create an `index.md` file inside each (copy from an existing publication as a template)
3. Set the `authors`, `date`, `publication`, `tags`, and `links` fields

### Update your CV PDF
Replace `static/uploads/resume.pdf` with your latest CV/Biosketch file.

### Update your headshot
Replace `assets/media/authors/me.jpg` with your photo.

### Update hero images (immunofluorescence/IHC)
Replace or add images in `static/media/hero/` and update the `<img>` tags in both `content/en/_index.md` and `content/zh/_index.md`.

## Project Structure

```
config/_default/        # Site configuration (hugo.yaml, params.yaml, languages.yaml, menus.yaml)
content/en/             # English content (_index.md, publications/, authors/)
content/zh/             # Chinese content (_index.md, publications/, authors/)
data/authors/me.yaml    # Author profile data (shared across languages)
assets/media/authors/   # Headshot photo
static/media/hero/      # Hero banner images (IF/IHC)
static/uploads/         # CV PDF
.github/workflows/      # GitHub Actions deployment
```

## Deployment

Auto-deploys to GitHub Pages via GitHub Actions on push to `main`. See `.github/workflows/deploy.yml`.

### Setup
1. Create repo `caotianyu0427/caotianyu0427.github.io` on GitHub
2. Push this code to `main` branch
3. In repo Settings → Pages, set Source to "GitHub Actions"

## Tech Stack

- **Hugo** v0.158.0+ (extended) — Static site generator
- **HugoBlox Academic CV** — Academic theme with publication management
- **GitHub Pages** — Hosting
- **GitHub Actions** — CI/CD
- **Bilingual** — English + Chinese with language switcher
