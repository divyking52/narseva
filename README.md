# Nar Seva Narayan Seva

Standalone charity website (Altruist-inspired layout) for [Nar Seva Narayan Seva](https://narsevanarayanseva.com/).

## Local preview

Open `index.html` in a browser, or:

```bash
python -m http.server 8877
```

## Deploy

Site deploys with GitHub Actions → GitHub Pages on every push to `main`.

### 1. Enable GitHub Pages (one-time)

1. Open https://github.com/divyking52/narseva/settings/pages  
2. Under **Build and deployment** → Source: **GitHub Actions**  
3. Wait for the **Deploy to GitHub Pages** workflow to finish (Actions tab)  
4. Site URL: https://divyking52.github.io/narseva/  

### 2. Point Hover DNS at GitHub Pages

In [Hover](https://www.hover.com/) → your domain → **DNS**:

| Type | Host | Value |
|------|------|--------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `divyking52.github.io` |

Then in GitHub Pages settings, set custom domain to `narsevanarayanseva.com` (a `CNAME` file is already in the repo). Remove any old Hover default A record that points elsewhere.
