# Su Mangale Portfolio (Hugo)

This is the source for Su Mangale's portfolio static site, built with [Hugo](https://gohugo.io/) and the [hello-friend-ng theme](https://github.com/rhazdon/hugo-theme-hello-friend-ng).

## Quick Start

1. **Install Hugo**
   - See: https://gohugo.io/getting-started/installing/

2. **Add the hello-friend-ng theme**
   ```bash
   git submodule add https://github.com/rhazdon/hugo-theme-hello-friend-ng.git themes/hello-friend-ng
   ```

3. **Copy the example config**
   ```bash
   cp themes/hello-friend-ng/exampleSite/config.toml ./config.toml
   ```

4. **Customize your content**
   - Edit `config.toml` for your name, social links, and site info.
   - Add your content in the `content/` directory (e.g., `about.md`, `posts/`, etc).

5. **Run locally**
   ```bash
   hugo server -D
   ```
   Visit http://localhost:1313

6. **Build for GitHub Pages**
   ```bash
   hugo --minify
   # The static site will be in the public/ directory
   ```

7. **Push to GitHub**
   - Commit and push the `public/` directory to the `main` branch of your `su-mangale.github.io` repo.
   - Enable GitHub Pages for the repo (set source to `/ (root)` or `/public` as needed).

---

## Directory Structure

```
su-mangale.github.io/
├── config.toml
├── content/
│   ├── _index.md
│   ├── about.md
│   └── posts/
├── themes/
│   └── hello-friend-ng/
└── public/
```

## Customization
- Update `config.toml` for your profile, social links, and theme options.
- Add posts or pages in `content/` to share your DevOps, Kubernetes, FluxCD, Nutanix, Jenkins, and Git experiences.

For more, see the [hello-friend-ng theme docs](https://github.com/rhazdon/hugo-theme-hello-friend-ng#readme).
