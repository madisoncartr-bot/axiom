# AXIOM.OS — Your Complete Launch Guide

Everything you need to get from these files to a live website. 
Estimated time: 20–30 minutes.

---

## What you have

Your site has 5 pages:
- `/` — Home (the landing page)
- `/brain` — Second Brain / Knowledge Base
- `/log` — Learning Log with subscribe box
- `/career` — Timeline + Projects
- `/now` — Now page (what you're focused on)

---

## Step 1 — Install the tools (5 min)

You need two things on your computer:

**Node.js** (the engine that runs your site locally):
1. Go to https://nodejs.org
2. Download the LTS version (big green button)
3. Install it (just click through the installer)

**Verify it worked** — open Terminal (Mac) or Command Prompt (Windows) and type:
```
node --version
```
You should see something like `v20.x.x`. Good.

---

## Step 2 — Set up your project (3 min)

1. Create a folder on your computer called `axiom-os`
2. Copy all the files from this download into that folder — your folder should look like:

```
axiom-os/
├── package.json
├── astro.config.mjs
├── public/
│   └── favicon.svg
└── src/
    ├── layouts/
    │   └── Base.astro
    ├── pages/
    │   ├── index.astro
    │   ├── brain.astro
    │   ├── log.astro
    │   ├── career.astro
    │   └── now.astro
    └── styles/
        └── global.css
```

3. Open your terminal, navigate to the folder:
```
cd axiom-os
```

4. Install dependencies:
```
npm install
```

5. Run locally to see it in your browser:
```
npm run dev
```

Open http://localhost:4321 — your site is running locally. 🎉

---

## Step 3 — Create a GitHub account (5 min)

GitHub is where your code lives. Vercel (the host) reads from it automatically.

1. Go to https://github.com
2. Click **Sign up**
3. Choose a username — this doesn't show on your site, but something like `yourinitials-dev` works
4. Verify your email

**Create a new repository:**
1. On GitHub, click the **+** button → **New repository**
2. Name it: `axiom-os`
3. Set it to **Public**
4. Click **Create repository**

**Upload your files:**
The easiest way with no Git knowledge:
1. On your new empty repo page, click **uploading an existing file**
2. Drag your entire `axiom-os` folder contents in
3. Click **Commit changes**

---

## Step 4 — Deploy to Vercel (5 min)

1. Go to https://vercel.com
2. Click **Sign Up** → choose **Continue with GitHub** (links your accounts)
3. Click **Add New Project**
4. Find `axiom-os` in your repository list → click **Import**
5. Vercel auto-detects it's an Astro project — leave all settings as-is
6. Click **Deploy**

Watch the build log run. In about 60 seconds you'll see:

```
✅ Deployment complete
```

Your site is live at: **`axiom-os.vercel.app`**

---

## Step 5 — Personalise your content (ongoing)

Now the fun part. Open your files and replace the placeholder content:

### `src/pages/index.astro`
- Update the terminal panel stats (notes, streak, what you're reading/building)

### `src/pages/brain.astro`
- Replace the 6 example notes with your actual mental models and ideas
- Add/remove tags to match your thinking

### `src/pages/log.astro`
- Replace the example posts with your actual writing
- Update the reading list and learning track progress bars

### `src/pages/career.astro`
- Replace the timeline with your actual career history
- Replace the projects with your real projects

### `src/pages/now.astro`
- This one is most important — write this in your own voice
- Update it at least once a month

---

## Updating your site (ongoing)

Every time you want to update content:

1. Edit the `.astro` file in your editor
2. Go to your GitHub repo → find the file → click the pencil icon to edit
3. Make your changes → click **Commit changes**
4. Vercel automatically re-deploys in ~60 seconds

No terminal needed after initial setup.

---

## Optional: Custom domain ($10–15/year)

Instead of `axiom-os.vercel.app`, get something like `axiom.so` or `yourname.xyz`:

1. Buy a domain at **Porkbun** (https://porkbun.com) — cheapest prices, great UI
2. In Vercel → your project → **Settings** → **Domains**
3. Type your domain → Vercel gives you DNS settings
4. In Porkbun → your domain → **DNS** → add the records Vercel shows you
5. Wait 10–30 minutes → your domain is live

---

## What to build next

Once you're live, here's what will make the site more powerful:

1. **Real blog posts** — write one post per week in the Learning Log
2. **More brain notes** — add 3-5 notes per week
3. **Newsletter** — connect your subscribe form to Buttondown or Beehiiv (both free)
4. **Analytics** — add Vercel Analytics (free, privacy-friendly) to see who's reading
5. **Search** — Astro has great search integrations (Pagefind is free and excellent)

---

## Need help?

- Astro docs: https://docs.astro.build
- Vercel docs: https://vercel.com/docs
- GitHub basics: https://docs.github.com/en/get-started

Good luck. Ship it. Then write about it in the Learning Log.

---

*AXIOM.OS — built in the open*
