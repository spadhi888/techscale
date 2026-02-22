# TechScale Website

Static site for techscaleglobal.com.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g., `techscaleglobal` or `techscaleglobal.github.io`).

2. Add the remote and push:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git add -A
   git commit -m "Initial commit"
   git branch -M main
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to **Settings → Pages**
   - Under **Source**, select **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)`
   - Click Save

4. Configure custom domain (techscaleglobal.com):
   - The `CNAME` file is already in the repo
   - In your domain DNS, add a CNAME record:
     - **Name:** `www` (or `@` for apex)
     - **Value:** `YOUR_USERNAME.github.io`
   - For apex (techscaleglobal.com), GitHub recommends A records; see [GitHub Pages custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

5. In GitHub Pages settings, enter `techscaleglobal.com` in the Custom domain field and enable **Enforce HTTPS** once DNS propagates.
