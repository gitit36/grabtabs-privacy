# Adding Terms of Service to GitHub Pages

To make your terms of service accessible at `privacy.onp0int.com/terms-and-conditions`, follow these steps:

## Option 1: If you have a GitHub Pages repository

1. **Navigate to your GitHub Pages repository** (the one hosting `privacy.onp0int.com`)

2. **Add the terms file**:
   - Upload `terms-and-conditions.html` to your repository
   - Or create a new file in your repository called `terms-and-conditions.html`
   - Copy the contents from the file we just created

3. **Commit and push**:
   ```bash
   git add terms-and-conditions.html
   git commit -m "Add terms of service page"
   git push
   ```

4. **Verify**:
   - Wait a few minutes for GitHub Pages to update
   - Visit: `https://privacy.onp0int.com/terms-and-conditions`
   - The page should load correctly

## Option 2: If you're using a custom domain with GitHub Pages

1. Make sure your `CNAME` file in the repository root contains:
   ```
   privacy.onp0int.com
   ```

2. Add `terms-and-conditions.html` to the root of your repository (same level as `index.html` or your privacy policy)

3. The URL will automatically be: `https://privacy.onp0int.com/terms-and-conditions`

## Option 3: If you need to create a new repository

1. **Create a new GitHub repository** (or use existing one)

2. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Select source branch (usually `main` or `gh-pages`)
   - Save

3. **Add files**:
   - Add `terms-and-conditions.html` to the repository root
   - Optionally add `index.html` that links to both privacy and terms

4. **Set up custom domain** (if not already done):
   - In repository Settings → Pages → Custom domain
   - Enter: `privacy.onp0int.com`
   - Add `CNAME` file to repository root with: `privacy.onp0int.com`

5. **Update DNS** (if needed):
   - Add CNAME record: `privacy` → `yourusername.github.io`

## Quick Setup Script

If you have the repository locally:

```bash
# Navigate to your GitHub Pages repository
cd /path/to/your/privacy-pages-repo

# Copy the terms file
cp /path/to/grabtab/grabtab_v6.1/terms-and-conditions.html .

# Commit and push
git add terms-and-conditions.html
git commit -m "Add terms of service page for Paddle integration"
git push origin main
```

## Verify It Works

After pushing, wait 1-2 minutes, then visit:
- `https://privacy.onp0int.com/terms-and-conditions`

You should see the terms of service page.

## For Paddle

Once the page is live, use this URL in Paddle:
```
https://privacy.onp0int.com/terms-and-conditions
```

This meets Paddle's requirement that the URL includes a path.

