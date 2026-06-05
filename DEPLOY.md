# Deploying this static blog

Quick options to publish the static site in this repository.

- **GitHub Pages (recommended for simple hosting)**

1. Create a GitHub repository and push this project:

```
git init
git add .
git commit -m "Add static blog site"
git branch -M main
git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

2. In the repository Settings → Pages, set the source to the `main` branch and root (`/`), then save. Your site will be available at `https://YOUR_USERNAME.github.io/YOUR_REPO/`.

- **Netlify or Vercel (recommended for custom domain + HTTPS)**

1. Sign in to Netlify or Vercel and choose "New site" → "Import from Git" and connect your GitHub repository.
2. For a static site with no build step, accept defaults and deploy.
3. In Netlify/Vercel dashboard you can add a custom domain and they will provide automatic HTTPS.

- **Custom domain (general steps)**

1. Buy a domain (Namecheap, Google Domains, etc.).
2. In your hosting dashboard add the custom domain.
3. Update DNS records at your registrar: for Netlify use the provided CNAME/ALIAS records; for GitHub Pages add an A record (points to GitHub Pages IPs) or a CNAME to yourusername.github.io.
4. Wait for DNS propagation (minutes to hours). Enable HTTPS if the host provides it.

If you'd like, I can:
- create a Git repo and push to GitHub (I will need your permission and a repo name),
- or connect the site to Netlify/Vercel for you (will need account/access). 
