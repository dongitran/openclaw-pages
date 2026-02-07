# openclaw-pages

GitHub Pages hosting for OpenClaw projects. Each folder becomes a separate GitHub Pages site.

## Structure

```
openclaw-pages/
├── AGENTS.md           # This file
└── {project-name}/     # Each project has its own folder
    └── index.html      # Entry point for GitHub Pages
```

## Creating a New Page

1. Create project folder: `mkdir {project-name}`
2. Add your files (index.html, styles, scripts, etc.)
3. Commit and push:
   ```bash
   git add . && git commit -m "feat: add {project-name}" && git push
   ```

## Enabling GitHub Pages for a Folder

After pushing, enable GitHub Pages in repo settings:
1. Go to **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `master`, folder: `/ (root)`
4. Each folder accessible at: `https://dongitran.github.io/openclaw-pages/{project-name}/`

## Rules

- One folder per project
- Each folder must have `index.html`
- Use relative paths for assets
- Pull before pushing to avoid conflicts
