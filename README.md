# Harikrishnan Aneesh — portfolio

A single static page: `index.html`, no build step. Fonts load from Google Fonts.

## Host it on your own domain

Pick one. All three serve the repo root as-is.

### GitHub Pages
1. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
2. Same page → Custom domain → enter your domain → Save (this creates a `CNAME` file).
3. At your DNS provider:
   - Apex domain (`example.com`): four `A` records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
   - `www`: a `CNAME` record → `<your-github-username>.github.io`.
4. Tick **Enforce HTTPS** once the certificate is issued.

### Vercel
Import the repo (Framework: Other, no build command, output `.`), then Settings → Domains → add your domain and follow the DNS records it shows.

### Netlify
Add new site → Import from Git → leave build command empty, publish directory `.`, then Domain management → add your domain.

## Update
Edit `index.html`, commit, push. The host redeploys automatically.
