# EditPro GitHub Pages Website

This folder contains the GitHub Pages website for EditPro, including the landing page and privacy policy.

## 🌐 Live URL

Once GitHub Pages is enabled, your site will be available at:
```
https://[your-github-username].github.io/EditPro/
```

Privacy Policy URL for App Store:
```
https://[your-github-username].github.io/EditPro/privacy.html
```

## 📁 Folder Structure

```
docs/
├── index.html          # Landing page
├── privacy.html        # Privacy policy (required for App Store)
├── style.css           # Shared CSS styles
├── .nojekyll           # Tells GitHub to skip Jekyll processing
├── assets/             # Assets folder
│   └── screenshots/    # Add app screenshots here
└── README.md           # This file
```

## 🚀 How to Enable GitHub Pages

1. Go to your EditPro repository on GitHub
2. Click **Settings** tab
3. Scroll to **Pages** section in the left sidebar
4. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: **main** (or **feat/release-prep**)
   - Folder: **/docs**
5. Click **Save**
6. Wait 2-3 minutes for deployment
7. Visit your site at the URL shown

## 📸 Adding Screenshots

To add app screenshots to the landing page:

1. Take screenshots on your iPhone (iOS screenshots)
2. Export them from your device
3. Optimize images (compress for web)
4. Add them to `docs/assets/screenshots/` folder
5. Update `index.html` to reference the images:

```html
<!-- Replace the placeholder divs with -->
<div class="screenshot">
    <img src="assets/screenshots/timeline-view.png" alt="Timeline View">
</div>
```

### Recommended Screenshot Sizes:
- Width: 400-600px (for web display)
- Format: PNG or JPG
- Optimize with tools like TinyPNG or ImageOptim

## 🎨 Adding the App Icon

1. Export your app icon (1024x1024px)
2. Save as `docs/assets/app-icon.jpg`
3. Update `index.html`:

```html
<!-- Find this section in index.html -->
<div class="app-icon-placeholder">
    <span class="icon-text">EditPro</span>
</div>

<!-- Replace with -->
<div class="app-icon">
    <img src="assets/app-icon.jpg" alt="EditPro App Icon">
</div>
```

4. Add CSS in `style.css`:

```css
.app-icon img {
    width: 300px;
    height: 300px;
    border-radius: 60px;
    box-shadow: 0 20px 60px rgba(139, 92, 246, 0.4);
}
```

## ✏️ Updating Content

### Update Privacy Policy

Edit `docs/privacy.html` and update the "Last Updated" date.

### Update Landing Page

Edit `docs/index.html`:
- Change "Coming Soon" to actual App Store link when published
- Add real screenshots
- Update feature descriptions
- Add testimonials or reviews

### Change Styling

Edit `docs/style.css` to customize:
- Colors (update CSS variables at the top)
- Layout
- Typography
- Responsive breakpoints

## 🔗 App Store Integration

When submitting to App Store Connect:

1. **Privacy Policy URL**:
   ```
   https://[your-username].github.io/EditPro/privacy.html
   ```

2. **Marketing URL** (optional):
   ```
   https://[your-username].github.io/EditPro/
   ```

3. **Support URL**:
   ```
   https://[your-username].github.io/EditPro/
   ```
   Or use: `mailto:dsoulkeeper@gmail.com`

## 🎯 Custom Domain (Optional)

To use a custom domain (e.g., `editpro.app`):

1. Buy domain from registrar (Namecheap, Google Domains, etc.)
2. Add DNS records:
   ```
   Type: CNAME
   Host: www
   Value: [your-username].github.io
   ```
3. Create `docs/CNAME` file with your domain:
   ```
   www.editpro.app
   ```
4. Push to GitHub
5. Enable HTTPS in GitHub Pages settings

## 📝 File Descriptions

### index.html
- Landing page for EditPro
- Showcases features, screenshots
- Links to App Store (when ready)
- Privacy-focused messaging

### privacy.html
- Complete privacy policy
- Apple-compliant language
- EditPro-specific (no tracking, local processing)
- Required for App Store submission

### style.css
- Purple gradient theme (#8B5CF6 to #6366F1)
- Mobile-responsive design
- Dark theme optimized
- Shared between both pages

### .nojekyll
- Empty file that tells GitHub to skip Jekyll processing
- Ensures faster builds and proper HTML serving

## 🔄 Updating the Site

Any time you push changes to the `docs/` folder:

```bash
git add docs/
git commit -m "Update website content"
git push
```

GitHub Pages will automatically rebuild and deploy within 2-3 minutes.

## 🐛 Troubleshooting

**Site not loading?**
- Check GitHub Pages is enabled in Settings
- Verify branch and folder are correct
- Wait 3-5 minutes after pushing changes
- Check for build errors in Settings → Pages

**Styles not applying?**
- Make sure `style.css` path is correct in HTML
- Clear browser cache (Cmd+Shift+R)
- Check browser console for errors

**Images not showing?**
- Use relative paths: `assets/screenshots/image.png`
- Not absolute paths: `/assets/screenshots/image.png`
- Ensure images are in the correct folder

## 📧 Support

For questions or issues:
- Email: dsoulkeeper@gmail.com
- Edit files and push updates anytime

---

**Next Steps:**
1. Enable GitHub Pages in repository settings
2. Add app screenshots to `assets/screenshots/`
3. Replace app icon placeholder
4. Update "Coming Soon" with real App Store link
5. Test the site on mobile devices

Good luck with your App Store submission! 🚀
