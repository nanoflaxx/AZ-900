# 🚀 Deploy to Netlify in 2 Minutes

## Fastest Option: Drag & Drop

1. **Go to** https://netlify.com (create free account if needed)
2. **Drag & drop** `az900_course.html` onto the Netlify dashboard
3. **Done!** Your site is live at a random URL like `https://xxx-yyy-123.netlify.app`

✅ Takes literally 30 seconds

---

## Better Option: Custom Domain + Auto-Deploy

1. **Create a GitHub repository** (free at github.com)
   ```
   az900-course/
   ├── az900_course.html
   ├── netlify.toml
   └── README.md
   ```

2. **Push your files to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

3. **Go to Netlify** → "New site from Git"
   - Connect GitHub
   - Select your `az900-course` repo
   - Netlify auto-detects config
   - Click "Deploy"

4. **Wait 30 seconds** ✅

5. **Add custom domain** (optional)
   - In Netlify, go Settings → Domain management
   - Add your domain or request a free Netlify subdomain

---

## What You Get

✨ **Free tier includes:**
- Unlimited sites
- HTTPS (SSL/TLS) automatic
- Global CDN (fast everywhere)
- Deploy previews for branches
- Environment variables if you need them later

---

## Files Explained

| File | Purpose |
|------|---------|
| `az900_course.html` | Your entire course (no dependencies) |
| `netlify.toml` | Tells Netlify how to serve your site |
| `README.md` | Full documentation |

---

## After Deployment

✅ Your course is live!
- Share the URL with students
- Netlify handles SSL/HTTPS automatically
- Updates are instant (just push to GitHub)
- Analytics available in Netlify dashboard

---

## Troubleshooting

**Q: I see a blank page**
- Check browser console (F12 → Console tab)
- Make sure HTML file is named exactly `az900_course.html`
- Verify `netlify.toml` is in repository root

**Q: How do I update the course?**
- Edit `az900_course.html` locally
- Push to GitHub
- Netlify auto-deploys in 30 seconds

**Q: Can I use a custom domain?**
- Yes! Add it in Netlify settings (Domain management)
- $12/year or bring your own

---

Need help? See `README.md` for detailed troubleshooting! 📖
