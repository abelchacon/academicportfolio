# GitHub Pages Setup Guide

## What's Included

This portfolio consists of:
- **index.html** - Main portfolio page with sections for About, Projects, and Contact
- **styles.css** - Responsive styling with modern design
- **.gitignore** - Standard web project ignores
- **SETUP.md** - This setup guide

## Customization

Before publishing, update the following in `index.html`:

1. **Name and Contact Info**
   - Replace "Abel Chacon" with your name
   - Update email, GitHub, and LinkedIn URLs in the Contact section

2. **About Section**
   - Edit the bio paragraph
   - Update skills list to match your expertise

3. **Projects**
   - Modify project titles and descriptions
   - Add project links

## Publishing to GitHub Pages

### Step 1: Prepare Your Repository
```bash
# Make sure you're in the repo directory
cd /path/to/academicportfolio

# Ensure all changes are committed
git add .
git commit -m "Initial portfolio setup"
git push origin main  # or master, depending on default branch
```

### Step 2: Configure GitHub Pages

1. Go to your repository on GitHub: https://github.com/abelchacon/academicportfolio
2. Click **Settings** tab
3. Scroll to **Pages** section (left sidebar)
4. Under "Source", select:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
5. Click **Save**

### Step 3: Wait for Deployment

GitHub will automatically build and deploy your site. You'll see:
- A green checkmark when deployment is complete
- Your site will be available at: `https://abelchacon.github.io/academicportfolio/`

## Monitoring Deployment

- Check deployment status: Settings → Pages
- View Actions tab to see build logs: https://github.com/abelchacon/academicportfolio/actions

## Next Steps

### Add More Pages
Create additional HTML files (e.g., `projects.html`, `blog.html`) and link them from the navigation.

### Enhance Styling
- Modify `styles.css` to match your brand
- Add images in an `assets/` or `images/` folder
- Update color scheme via CSS variables (`:root` in styles.css)

### Add Custom Domain (Optional)
In GitHub Settings → Pages, you can point a custom domain to your site.

## Troubleshooting

**Site not showing up:**
- Confirm Settings → Pages shows green checkmark
- Clear browser cache (Ctrl+Shift+Del / Cmd+Shift+Del)
- Wait 1-2 minutes for DNS to propagate

**Style not loading:**
- Ensure `styles.css` is in the root directory
- Check browser console (F12) for 404 errors
- Verify relative paths in HTML

**Need to unpublish?**
- Settings → Pages → Source → "None"
- Site will be removed after ~10 minutes
