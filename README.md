# Learn

Static study apps, one folder per subject, published together to GitHub Pages by `.github/workflows/deploy.yml`:

| Folder | App | Source project |
|---|---|---|
| `maths/` | Maths Explorer (CBSE Maths, Grades 3–10) | `../maths-explorer` (`npm run publish:learn`) |

Each subject is served at `/<repo>/<subject>/`, for example `/learn/maths/`.

**To add a subject:** build the app with a relative base (`base: './'` in Vite) so it works from any sub-path. Copy its build output into a new folder here (for example `physics/`), then commit and push to `main`. There is no root page: each subject is opened directly at its own path. The workflow publishes every folder that contains an `index.html`.

---

