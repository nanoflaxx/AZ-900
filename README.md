# AZ-900 Azure Fundamentals — Complete Interactive Course

A fully-featured, self-contained interactive learning course for the Microsoft AZ-900 exam with built-in assessment test.

## ✨ Features

- 📚 **4 Complete Modules** covering all AZ-900 exam objectives
- 15 Interactive lessons with Learn, Analogy, and Quiz tabs
- 🧪 **Assessment Test** — choose 25, 50, or 70 random questions from a bank of 200
- 📊 **Probability Score** — get an exam readiness percentage
- 🔗 **Resource Links** — organized by topic for quick study reference
- 🌓 **Dark Mode** — automatic system preference detection
- 📱 **Fully Responsive** — works on desktop, tablet, and mobile
- ⚡ **Zero Dependencies** — single HTML file, no backend needed

## 🚀 Deploy to Netlify

### Option 1: Drag & Drop (Easiest)

1. Go to [Netlify.com](https://netlify.com)
2. Sign in or create a free account
3. Drag the `az900_course.html` file directly onto the Netlify dashboard
4. ✅ Done! Your site is live

### Option 2: Git Integration (Recommended)

1. Create a new GitHub repository
2. Upload these files:
   - `az900_course.html` (your course file)
   - `netlify.toml` (configuration)
   - `README.md` (this file)

3. Go to [Netlify.com](https://netlify.com) → "New site from Git"
4. Connect your GitHub account
5. Select your repository
6. Netlify auto-detects the config and deploys automatically ✅

### Option 3: Netlify CLI (For developers)

```bash
# Install Netlify CLI globally
npm install -g netlify-cli

# Login to your Netlify account
netlify login

# Deploy the directory
netlify deploy --prod --dir=.
```

## 📝 File Structure

```
your-repo/
├── az900_course.html    ← Main course file (no need to rename)
├── netlify.toml         ← Netlify config (tells Netlify how to serve)
└── README.md            ← This file
```

## 🎯 How It Works

### Learning Mode
- Select a module to start learning
- Each lesson has three tabs: **Learn**, **Analogy** (for memory), and **Quiz**
- Complete all lessons to unlock module completion badges
- Track your progress with the dashboard

### Assessment Test
- Click the **Assessment Test** tab
- Choose test length: 25️⃣ / 50️⃣ / 70️⃣ questions
- Answer questions (you can change answers anytime)
- Submit to see your score and **exam readiness probability**
- Review resource links to study weak areas
- Take another test to track progress

## ⚖️ Important Disclaimer

**⚠️ This practice test does NOT guarantee you'll pass the official Microsoft AZ-900 exam.**

The assessment is designed to:
- ✅ Help identify knowledge gaps
- ✅ Build exam confidence
- ✅ Provide study guidance

But remember:
- The real exam may cover different topics with different emphasis
- Question formats may differ
- You need comprehensive study with official Microsoft resources

**Always refer to the official [Microsoft AZ-900 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900)** for complete exam objectives.

## 🎨 Customization

The course uses CSS variables for easy theming. Edit the `:root` section in the `<style>` tag:

```css
:root {
  --bg: #fff;           /* Background color */
  --txt: #1a1a18;       /* Text color */
  --acc: #185FA5;       /* Accent color (blue) */
  --ok: #3B6D11;        /* Success color (green) */
  /* ... more variables ... */
}
```

Dark mode is automatic — the browser's `prefers-color-scheme` media query handles it.

## 📊 Question Bank

The test includes 200 questions covering:
- Azure fundamentals & cloud concepts
- Compute services (VMs, App Service, Functions, Containers)
- Storage solutions (Blob, SQL, Cosmos DB, Data Lake)
- Networking & Security (VNets, NSGs, Firewall, Key Vault)
- Management & Governance (Policy, ARM, Cost Management)
- Monitoring & Analytics (Azure Monitor, Application Insights, Log Analytics)

Questions are **randomly shuffled** each test — no two tests are identical.

## 🔗 Resource Links Included

- Microsoft Azure Documentation
- Azure Pricing Calculator
- Official AZ-900 Study Guide
- Free Official Practice Assessment
- Exam sandbox to try the real interface
- Exam accommodations request (extra time, etc.)

Plus module-specific links like:
- VM Docs, App Service, Functions, Container Instances
- Blob Storage, SQL Database, Cosmos DB
- Virtual Networks, Firewall, Key Vault
- Policy, Resource Manager, Cost Management
- Azure Monitor, Application Insights, Log Analytics

## 💾 Local Testing

Before deploying, test locally:

1. Download `az900_course.html`
2. Right-click → "Open with" → your browser
3. Or run a local server: `python -m http.server` (Python 3)
4. Visit `http://localhost:8000/az900_course.html`

## 🐛 Troubleshooting

### Q: The course won't load on Netlify
**A:** Make sure the `netlify.toml` file is in your repository root and the HTML file is named exactly `az900_course.html`

### Q: Dark mode isn't working
**A:** This is automatic based on your system preferences. Check your OS/browser dark mode setting.

### Q: Can I edit the questions?
**A:** Yes! Open the HTML file in a text editor, find the `QUESTIONS` array (around line 909), and modify or add questions. Keep the format consistent: `{q:"question text", opts:[...], answer: 0}`

### Q: My answers aren't saving
**A:** This is by design — answers are stored in memory during the test session. They reset when you refresh or restart the test. If you want persistent storage, you'd need to add a backend (database).

## 📈 Future Enhancements

Possible improvements:
- Answer history/progress tracking (localStorage)
- Timed tests (countdown timer)
- Question difficulty indicators
- Performance analytics dashboard
- Export test results as PDF

## 📄 License

This course material is provided as-is for educational purposes. Microsoft Azure, Azure Fundamentals, and AZ-900 are trademarks of Microsoft Corporation.

## 🙋 Support

For issues or questions:
1. Check the **Troubleshooting** section above
2. Review the code comments in `az900_course.html`
3. Check [Netlify docs](https://docs.netlify.com/)
4. Visit [Microsoft Learn](https://learn.microsoft.com/en-us/azure/) for exam prep help

---

**Happy studying! 🚀 Good luck with your AZ-900 exam!**
