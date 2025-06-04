# Mangale Portfolio & Blog (Markdown-Only, GitHub Pages)

This is the source for Su Mangale's personal portfolio and blog, built using only Markdown files and GitHub Pages' built-in Jekyll support. No HTML, CSS, or static site generator is required.

## How It Works
- All content is written in Markdown (`.md`) files.
- Blog posts are placed in the `_posts/` directory, following the format `YYYY-MM-DD-title.md`.
- GitHub Pages automatically builds and publishes the site using Jekyll.
- The default Jekyll theme is used (can be changed in repository settings if desired).

## Directory Structure
```
su-mangale.github.io/
├── _posts/
│   └── 2025-06-04-fluxcd-gitops-getting-started.md
├── about.md
├── index.md
├── LICENSE
└── README.md
```

## Adding Content
- **Homepage:** Edit `index.md`.
- **About page:** Edit `about.md`.
- **Blog posts:** Add new markdown files to `_posts/` with the format `YYYY-MM-DD-title.md` and YAML front matter, e.g.:
  ```markdown
  ---
  title: "My New Post"
  date: 2025-06-04
  ---
  Your content here.
  ```

## Publishing
1. Commit and push your changes to the `main` branch of this repository.
2. GitHub Pages will automatically build and publish your site at `https://<your-username>.github.io/`.

## Customization
- You can change the Jekyll theme in the repository's GitHub Pages settings.
- No HTML or CSS editing is required, but you can add customizations if desired.

---

For more information, see the [GitHub Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages) and [Jekyll documentation](https://jekyllrb.com/docs/).
