# Lone Star Tax Save — GitHub Pages Starter

This is a simple static landing page designed for GitHub Pages.

## Files

- `index.html` — main page
- `styles.css` — styling
- `script.js` — tiny JS for footer year
- `404.html` — fallback page
- `CNAME` — custom domain file for `lonestartaxsave.com`
- `.nojekyll` — prevents Jekyll processing

## Quick deploy on GitHub Pages

1. Create a new GitHub repository, for example: `lonestartaxsave-site`
2. Upload all files from this folder to the repository root
3. On GitHub, go to **Settings → Pages**
4. Under **Build and deployment**, choose **Deploy from a branch**
5. Select your main branch and the **/(root)** folder
6. Save
7. In the same Pages screen, set the custom domain to:

   `lonestartaxsave.com`

8. Wait for GitHub Pages to publish
9. After DNS is correct and the certificate is ready, enable **Enforce HTTPS**

## DNS setup for the root domain

At your domain registrar / DNS provider, add these `A` records for `@`:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional IPv6 `AAAA` records:

- `2606:50c0:8000::153`
- `2606:50c0:8001::153`
- `2606:50c0:8002::153`
- `2606:50c0:8003::153`

## Recommended `www` setup

GitHub recommends also setting up the `www` version.

Add a `CNAME` record:

- Host: `www`
- Value: `YOUR-GITHUB-USERNAME.github.io`

Use your actual GitHub username only, not the repository name.

## Before launch

Search and replace these placeholders in `index.html`:

- `replace-me@lonestartaxsave.com`
- `(000) 000-0000`
- Any service descriptions you want to customize

## Migrating later to Railway

That is totally fine.

When you move to Railway later:

1. Deploy your app on Railway
2. Add `lonestartaxsave.com` and `www.lonestartaxsave.com` in Railway
3. Update DNS from GitHub Pages records to Railway’s target records
4. Keep the same domain and page URLs as much as possible

This makes GitHub Pages a good temporary landing page while you validate the content and branding.
