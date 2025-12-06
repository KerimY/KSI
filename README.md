# KSI Production Website

A modern, single-page React landing page for KSI Production.

## Features

- Responsive design (mobile-first)
- Smooth scroll navigation
- Animated sections with Framer Motion
- Contact form
- Upcoming events/casting section
- Job listings
- Social media integration

## Local Development

```bash
npm install
npm run dev
```

## Build for Production

```bash
npm run build
npm run preview
```

## Deployment with GitHub Pages (Free)

### Step 1: Create GitHub Repository

1. Go to github.com and create a new repo (e.g., `ksi-production`)
2. Don't initialize with README

### Step 2: Push Your Code

```bash
cd ksi-production
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ksi-production.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repo **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. Push any commit to trigger the deployment
4. Your site will be live at: `https://YOUR_USERNAME.github.io/ksi-production/`

The workflow file (`.github/workflows/deploy.yml`) is already included.

### Custom Domain

To use `ksi-production.com`:
1. Settings → Pages → Custom domain → enter your domain
2. At your DNS provider, add:
   - CNAME: `www` → `YOUR_USERNAME.github.io`
   - Or A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

## Alternative: Cloudflare Pages

1. Push to GitHub
2. Go to [Cloudflare Pages](https://pages.cloudflare.com)
3. Connect repo, set build command to `npm run build`, output to `dist`
4. Deploy - get a free `.pages.dev` URL

## Tech Stack

- React 18
- Vite
- Framer Motion
- Custom CSS

## Customization

- **Events**: Edit `upcomingEvents` array in `App.jsx`
- **Jobs**: Edit job listings in the Work section
- **Colors**: Update CSS variables in `:root` in `App.css`
