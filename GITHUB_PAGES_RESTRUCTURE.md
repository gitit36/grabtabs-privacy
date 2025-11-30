# Restructuring privacy.onp0int.com

## Current Structure
- `index.html` = Privacy Policy
- `terms-and-conditions.html` = Terms of Service

## New Structure
- `index.html` = Landing page (links to both policies)
- `privacy.html` = Privacy Policy
- `terms-and-conditions.html` = Terms of Service

## Steps to Update

1. **Backup your current `index.html`** (it's your privacy policy)

2. **Upload the new files to your GitHub Pages repository**:
   - `index.html` (new landing page)
   - `privacy.html` (moved from old index.html, updated)
   - `terms-and-conditions.html` (already exists, updated with navigation)

3. **Commit and push**:
   ```bash
   git add index.html privacy.html terms-and-conditions.html
   git commit -m "Restructure site: add landing page, move privacy to /privacy"
   git push
   ```

4. **Wait 1-2 minutes** for GitHub Pages to update

5. **Verify the URLs**:
   - `https://privacy.onp0int.com` → Landing page
   - `https://privacy.onp0int.com/privacy` → Privacy Policy
   - `https://privacy.onp0int.com/terms-and-conditions` → Terms of Service

## File Structure

```
your-repo/
├── index.html                    # Landing page
├── privacy.html                  # Privacy Policy
└── terms-and-conditions.html     # Terms of Service
```

## Navigation

All pages now have navigation links:
- Landing page links to both policies
- Privacy page links to home and terms
- Terms page links to home and privacy

## For Paddle

Use these URLs in Paddle settings:
- **Privacy Policy**: `https://privacy.onp0int.com/privacy`
- **Terms of Service**: `https://privacy.onp0int.com/terms-and-conditions`

Both URLs include paths as required by Paddle.

