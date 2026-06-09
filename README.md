# 🏗️ Lab: CI/CD with GitHub Actions + Netlify

## What you will build
A pipeline that automatically deploys a financial calculator to a public URL every time you do a `git push`.

## 🔗 Live URL
https://calculadorafinancierapr.netlify.app

---

## Requirements
- GitHub account
- Netlify account (free)
- Git installed
- VS Code installed

---

## Repository structure

lab-calculadora-hipoteca/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── index.html
├── netlify.toml
└── README.md

---

## Exercise phases

### Phase 1 — Push the project to GitHub
1. Create a repo on GitHub
2. Initialize locally
3. Add `index.html`
4. Run `git push`

### Phase 2 — Connect to Netlify
1. Create a Netlify account with GitHub
2. Import the repo
3. Automatic deploy
4. Verify the public URL

### Phase 3 — Add security headers
1. Create `netlify.toml` with security headers
2. Run `git push`
3. Check score at https://observatory.mozilla.org

### Phase 4 — GitHub Actions
1. Create `.github/workflows/deploy.yml`
2. Configure secrets in GitHub
3. Run `git push`
4. Watch the pipeline run in the Actions tab

---

## Required GitHub secrets

| Secret | Where to get it |
|---|---|
| `NETLIFY_AUTH_TOKEN` | Netlify → User settings → Personal access tokens |
| `NETLIFY_SITE_ID` | Netlify → Site configuration → Project ID |

---

## Final test
Make a change in `index.html`, run `git push` and observe:
1. The workflow running in GitHub → Actions tab
2. The updated URL on Netlify

---

## Security score
| Before | After |
|---|---|
| C (50/100) | B+ (80/100) |