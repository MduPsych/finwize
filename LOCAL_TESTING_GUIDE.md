# How to Run FinWise Locally (Before Hosting)

## ⚠️ Issue: file:// Protocol Error

When you open the HTML file directly from disk, you get:
```
Unsafe attempt to load URL file:///C:/Users/...
'file:' URLs are treated as unique security origins
```

This is a **browser security feature** - it prevents local HTML files from using localStorage.

## ✅ Solution 1: Use a Simple Local Server (EASY)

### Python 3 (Built-in):
```bash
# Navigate to the folder with finwise_complete.html
cd C:\Users\mduduzi.msiza\Downloads

# Run Python server
python -m http.server 8000

# Open browser
http://localhost:8000/finwise_complete.html
```

### Python 2:
```bash
cd C:\Users\mduduzi.msiza\Downloads
python -m SimpleHTTPServer 8000
# Then open: http://localhost:8000/finwise_complete.html
```

### Node.js:
```bash
# Install http-server globally (one time)
npm install -g http-server

# Navigate to folder
cd C:\Users\mduduzi.msiza\Downloads

# Start server
http-server

# Open: http://localhost:8080
```

### VSCode Live Server (Easiest if you have VSCode):
```
1. Open finwise_complete.html in VSCode
2. Right-click → "Open with Live Server"
3. Browser opens automatically
4. Works perfectly!
```

---

## ✅ Solution 2: Deploy to Free Hosting (BEST)

Skip local testing and deploy directly to GitHub Pages (5 minutes):

```
1. Create GitHub account: github.com/signup
2. Create repo: github.com/new → "finwise-app"
3. Upload: finwise_complete.html
4. Rename to: index.html
5. Enable Pages: Settings → Pages → main branch
6. Live at: https://YOUR-USERNAME.github.io/finwise-app/
```

No setup needed, works everywhere, free forever.

---

## ✅ Solution 3: Use an Online Editor

Copy-paste your code into:
- **Replit.com** - Free online IDE
- **CodePen.io** - Free online code editor
- **JSFiddle.net** - Free code playground

---

## Recommended: Deploy to GitHub Pages (No Local Testing Needed!)

Since the app is ready to use, just deploy it:

```
Step 1: Create GitHub Account (2 min)
└─ github.com/signup
└─ Verify email

Step 2: Create Repository (1 min)
└─ github.com/new
└─ Name: finwise-app
└─ Public
└─ Create

Step 3: Upload File (1 min)
└─ Click "Add file" → "Upload files"
└─ Drag finwise_complete.html
└─ Commit

Step 4: Enable Pages (1 min)
└─ Settings → Pages
└─ Branch: main
└─ Folder: / (root)
└─ Save

Step 5: Access Your App (immediately)
└─ Go to: https://YOUR-USERNAME.github.io/finwise-app/
└─ It works!
└─ Bookmark it
└─ Use daily
```

**That's it! Your app is live and works perfectly.**

---

## If You Want to Test Locally First

### Quick Test (Python Method - Recommended):

```bash
# Step 1: Open Command Prompt/Terminal
# Windows: Right-click → "Open PowerShell here"
# Mac/Linux: Right-click → "Open Terminal"

# Step 2: Check if Python is installed
python --version

# Step 3: Start server
python -m http.server 8000

# Step 4: Open browser
http://localhost:8000/finwise_complete.html

# Step 5: Test the app
# Add transactions, check updates
# Everything should work!

# Step 6: Stop server (when done)
# Press Ctrl+C in terminal
```

### With VSCode Live Server:

```
1. Download VSCode: code.visualstudio.com
2. Open finwise_complete.html in VSCode
3. Right-click → "Open with Live Server"
4. Browser opens automatically
5. Tests work perfectly
6. Auto-refreshes when you make changes
```

---

## Troubleshooting

### "Python not found"
- Install Python: python.org
- Choose "Add to PATH"
- Restart terminal
- Try again

### "Port 8000 already in use"
- Use different port: `python -m http.server 8001`
- Or: `http://localhost:8001/finwise_complete.html`

### "Cannot GET /"
- Make sure you're in the correct folder
- Make sure finwise_complete.html is in that folder
- Check with: `dir` (Windows) or `ls` (Mac/Linux)

### App won't save data
- Make sure you're using HTTP (http://localhost:8000)
- Not file:// protocol
- Data only works over HTTP/HTTPS

### localStorage still not working
- Try incognito/private window
- Check browser settings → privacy
- Make sure cookies are enabled
- Try different browser (Chrome, Firefox, etc.)

---

## Best Practice: Deploy Now

**Don't test locally - deploy to GitHub Pages now:**

1. ✅ Takes 5 minutes
2. ✅ Completely free
3. ✅ Works everywhere
4. ✅ No setup needed on your computer
5. ✅ Works on mobile
6. ✅ Works offline after first load

**Then use your live URL:**
```
https://YOUR-USERNAME.github.io/finwise-app/

Bookmark it → Use daily → Never worry about setup
```

---

## Summary

| Method | Time | Cost | Notes |
|--------|------|------|-------|
| **GitHub Pages** | 5 min | FREE | ⭐ Recommended |
| Python Server | 2 min | FREE | For local testing |
| VSCode Live Server | 1 min | FREE | If you have VSCode |
| Node http-server | 3 min | FREE | If you have Node |
| Netlify | 3 min | FREE | Alternative hosting |

**Go with GitHub Pages. Deploy now. Use forever.** 🚀

---

## Quick Deploy (Copy-Paste)

### Step 1: Open GitHub
```
github.com/signup
(Create account, verify email)
```

### Step 2: Create Repo
```
github.com/new
Name: finwise-app
Create repository
```

### Step 3: Upload File
```
Click "Add file" → "Upload files"
Select finwise_complete.html
Commit
```

### Step 4: Enable Pages
```
Settings → Pages
Branch: main
Folder: / (root)
Save
```

### Step 5: Use Your App
```
https://YOUR-USERNAME.github.io/finwise-app/
```

**Done! Your app is live.** 🎉

---

## Questions?

**Local testing not working?**
→ Just deploy to GitHub Pages instead (faster, easier)

**Want to test first?**
→ Use Python: `python -m http.server 8000`

**Need help deploying?**
→ See FREE_HOSTING_GUIDE.md

**App won't load?**
→ Check browser console (F12)
→ Look for errors
→ Make sure index.html is the filename

**Data not saving?**
→ Must be over HTTP/HTTPS (not file://)
→ Use local server or GitHub Pages

---

## Final Answer: Just Deploy to GitHub Pages

It's the fastest way:
1. Create account (1 min)
2. Create repo (1 min)
3. Upload file (1 min)
4. Enable Pages (1 min)
5. Your app is live (1 min)

**Total: 5 minutes, FREE forever, works everywhere.**

Stop overthinking. Deploy now. Use later. 🚀
