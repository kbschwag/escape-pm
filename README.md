# Escape WD — Project Manager

Your branded project management app. One HTML file, zero dependencies, free to deploy.

---

## 🚀 Deploy to Vercel (free, 5 minutes)

### Step 1 — Push to GitHub
1. Go to [github.com](https://github.com) and create a free account if you don't have one
2. Click **New repository** → name it `escape-pm` → Create
3. Upload `index.html` to the repo (drag and drop works)

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click **Add New Project** → Import your `escape-pm` repo
3. Click **Deploy** — done!

You'll get a live URL like `https://escape-pm.vercel.app`

---

## 👥 Sharing with your partner

Both of you visit the same Vercel URL. Tasks and clients save to shared storage automatically — no extra setup needed.

---

## 🔐 Client portal

Each client gets:
- The same URL + `#client-portal` appended (e.g. `https://escape-pm.vercel.app/#client-portal`)
- Their own email + password (you set these when adding a client)

They'll see:
- Their project progress bar
- Their tasks and milestones
- Attached documents
- A comment box to leave notes and upload files

---

## ✏️ Customizing

All styles are CSS variables at the top of `index.html`. To change the purple:
```css
--purple: #3d2b8e;        /* main purple */
--purple-dark: #2a1d6e;   /* hover state */
--accent: #7c5dfa;        /* accent purple */
```

---

## 📦 What's included

- **Tasks** — with assignment, recurring, priority, client linking
- **Calendar** — monthly view of all due dates
- **Clients** — cards with progress bars and portal preview
- **Artifacts** — link documents to clients and tasks
- **Client Portal** — password-protected dashboard per client
- **Shared storage** — team data syncs between you and your partner
