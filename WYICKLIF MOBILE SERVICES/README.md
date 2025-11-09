# Wyicklif Mobile Services — publish-ready

This repository contains your static site. To make the website visible on the public internet we prepared a `docs/` folder with the site content and a GitHub Actions workflow that can publish the `docs/` folder to GitHub Pages automatically.

What we added for you

- `docs/index.html`, `docs/service.html` — site pages ready to serve
- `docs/css/STYLE.css` — stylesheet adjusted for the `docs/` location
- `docs/assets/images/` — place your images here (we didn't include binary images)
- `.github/workflows/deploy-pages.yml` — workflow that uploads `docs/` and deploys Pages when you push to `main`.

Quick options to publish (pick one)

A) Publish using GitHub Pages (recommended)

1. Create a new GitHub repository (e.g. `wyicklif-site`).
1. From your project root (where this README is), run:

```powershell
cd "c:\HTML\work flow"
git init
git add .
git commit -m "Initial site for wyicklif"
# create remote (replace <your-username> and repo name):
git remote add origin https://github.com/<your-username>/wyicklif-site.git
git branch -M main
git push -u origin main
```

1. On GitHub: open the repo Settings → Pages. The included workflow will also deploy automatically after you push. If you prefer manual Pages, set Source to `main / docs` and save.

B) Publish using Netlify (very simple)

- Visit the Netlify site and sign up: [Netlify](https://app.netlify.com/)
- Create a new site from Git → choose your GitHub repo
- Set the build settings to publish directory: `docs` (no build command needed for static files)
- Deploy — Netlify will give you a public URL.

C) Quick temporary test (no push) — drag & drop

- Zip the contents of `docs/` or open `docs/` in Explorer and drag files into Netlify Drop: [Netlify Drop](https://app.netlify.com/drop). Netlify will host it instantly.

Notes & next steps

- Add your real images into `docs/assets/images/` (the stylesheet expects `wyicklif11.jpeg` at this path).
- If you want a custom domain, get a domain and configure DNS per GitHub Pages/Netlify instructions (I can help set DNS records).
- If you prefer I can also create a `CNAME` or help with Let's Encrypt on Netlify.

How I can help next

- I can walk you through creating the GitHub repo and running the push commands.
- I can help map a custom domain if you already own one.
- I can deploy to another platform (Firebase Hosting, Vercel, etc.) if you prefer.
