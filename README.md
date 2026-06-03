# Miao Xu Academic CV Website

This is a customized HugoBlox **Academic CV** website source package for summer research applications.
It is based on the current HugoBlox Academic CV template structure: `data/authors/me.yaml`, `assets/media/authors/me.png`, landing-page blocks, and Hugo modules.

## What has been filled in

- Personal profile and research direction
- Education, research experience, skills, awards, and languages
- Selected projects from the CV
- Publication page for **COVER: cross-vehicle transition framework for quadrotor control in air-ground cooperation**
- Profile photo at `assets/media/authors/me.png`
- Downloadable CV at `static/uploads/resume.pdf`
- GitHub Pages workflow at `.github/workflows/hugo.yaml`
- Netlify deployment config at `netlify.toml`

## Important placeholders to update before publishing

Primary profile data and public links are maintained in `data/authors/me.yaml`.

The current public contact email is `mi1070xu-s@student.lu.se`.

Open `config/_default/hugo.yaml` and replace:

```yaml
baseURL: 'https://your-github-username.github.io/'
```

If the repository will be named `username.github.io`, use:

```yaml
baseURL: 'https://username.github.io/'
```

If the repository will be named `academic-cv`, use:

```yaml
baseURL: 'https://username.github.io/academic-cv/'
```

## Local preview

Install Hugo Extended, Go, Node.js, and pnpm. Then run:

```bash
pnpm install --no-frozen-lockfile
hugo server --disableFastRender
```

Open the local URL printed by Hugo, usually:

```text
http://localhost:1313/
```

## Build

```bash
hugo --gc --minify
```

The generated site will be in `public/`.

## Deploy with GitHub Pages

1. Create a GitHub repository.
2. Push all files in this folder to the repository.
3. In GitHub, go to **Settings → Pages → Build and deployment**.
4. Select **GitHub Actions** as the source.
5. Push to `main`; the workflow will build and deploy the site.

## Deploy with Netlify

1. Create a new Netlify site from the GitHub repository.
2. Netlify will read `netlify.toml`.
3. Set the build command to `pnpm install --no-frozen-lockfile && hugo --gc --minify -b $URL` if Netlify does not auto-detect it.

## Notes

The package intentionally keeps content in Markdown/YAML so it is easy to edit.
If you later add GitHub, Google Scholar, ORCID, project videos, code links, or a personal statement, update the relevant files under `data/authors/`, `content/projects/`, and `content/publications/`.
