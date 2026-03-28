# Deploy to Vercel via GitHub (5 Minutes)

Vercel wants you to connect via GitHub. This is actually **better** because you can update your site anytime by just editing files on GitHub!

## Step 1: Create GitHub Repository (2 minutes)

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `dyoe-way`
3. Set to **Public** (required for free Vercel)
4. ✅ Check "Add a README file"
5. Click **"Create repository"**

---

## Step 2: Upload Your Files (2 minutes)

You have two options:

### Option A: Drag & Drop (Easiest)

1. In your new GitHub repo, click **"Add file"** → **"Upload files"**
2. Drag these files from your downloads:
   - `index.html`
   - `README.md`
   - `.gitignore`
   - (optionally: `instagram-posts.md`, `pitch-deck.md`, etc. for reference)
3. Click **"Commit changes"**

### Option B: GitHub Desktop (If you have it)

1. Clone your repo
2. Copy files into the folder
3. Commit and push

---

## Step 3: Connect to Vercel (1 minute)

1. Go back to [vercel.com](https://vercel.com)
2. Click **"Add New Project"**
3. Click **"Import"** next to your `dyoe-way` repository
4. Click **"Deploy"** (no settings needed)
5. **Done!** 🎉

---

## Your Live Site

Vercel will give you:
- **Preview URL:** `https://dyoe-way.vercel.app`
- **Custom domain option** (add your own domain in settings)

---

## Update Your Site Anytime

To change anything on your site:

1. Go to your GitHub repo
2. Click on `index.html`
3. Click the **pencil icon** (edit)
4. Make your changes
5. Click **"Commit changes"**
6. **Vercel auto-deploys in 10 seconds!** 🚀

No need to re-upload or redeploy manually.

---

## After Deployment

Once live, follow these steps from `DEPLOYMENT-README.md`:

1. **Set up Formspree** → Get form ID → Edit `index.html` on GitHub → Replace `YOUR_FORMSPREE_ID`
2. **Create Stripe payment links** → Edit `index.html` → Replace `STRIPE_STARTER_LINK` and `STRIPE_FULL_SERVICE_LINK`
3. **Start marketing** → Use `instagram-posts.md` and `cold-outreach-scripts.md`

---

## Files to Upload to GitHub

**Required:**
- ✅ `index.html` (your landing page)
- ✅ `README.md` (repo description)
- ✅ `.gitignore` (git settings)

**Optional (for your reference):**
- `instagram-posts.md`
- `pitch-deck.md`
- `cold-outreach-scripts.md`
- `stripe-integration-guide.md`
- `form-automation-guide.md`
- `DEPLOYMENT-README.md`

You can upload everything if you want, but only `index.html` is needed for the site to work.

---

## Need Help?

**GitHub Issues:**
- Make sure repo is **Public** (Vercel free tier requires this)
- If you can't find your repo in Vercel, refresh the import page

**Vercel Issues:**
- Make sure you gave Vercel permission to access your GitHub repos
- Click "Adjust GitHub App Permissions" if repo doesn't show up

---

## You're Ready!

5 minutes to live site. Then add your form and payment integration. Then start sending outreach messages.

Let's go! 🔥
