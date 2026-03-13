# Escape WD — Project Manager

Your branded client & project management app. One HTML file, zero dependencies, free to host.

---

## 🚀 Updating your live site

Every time you get a new `index.html` from Claude:

1. Go to **github.com/kbschwag/escape-pm**
2. Click `index.html` in the file list
3. Click the **pencil icon** (top right of the file view) to edit
4. Delete all the existing content and paste in the new file — OR click the upload button to replace it
5. Click **Commit changes**
6. Netlify auto-deploys in ~7 seconds ✓

Your live URL: **`benevolent-snickerdoodle-09b741.netlify.app`**

---

## 🔐 Client portal

Each client gets their own login. Here's how it works:

**Setting up a client:**
1. In your dashboard, go to **Clients** → **+ Add client**
2. Fill in their name, company, and project name
3. Set their **portal email** and **portal password** — you choose these
4. Add tasks and mark which ones are **"Visible on client dashboard"**

**Sharing with a client:**
- Send them your URL with `#client-portal` added to the end
- Example: `benevolent-snickerdoodle-09b741.netlify.app/#client-portal`
- They log in with the email and password you set
- They'll see their project progress, tasks, milestones, attached documents, and a comment box

**What clients can do:**
- View task progress and milestones (read-only)
- Leave comments and questions
- Attach files via the upload box

---

## 📋 Features

| Feature | Details |
|---|---|
| **Tasks** | Assign to you or partner, set priority, due date, recurring schedule |
| **Recurring tasks** | Daily / Weekly / Every 2 weeks / Monthly / Quarterly — auto-rolls forward when checked off |
| **Calendar** | Monthly view of all upcoming due dates, color-coded by project type |
| **Clients** | Cards with live progress bars, portal preview, copy login link |
| **Artifacts** | Save proposals, reports, and docs linked to clients and tasks |
| **Client Portal** | Password-protected dashboard per client with comments and file uploads |

---

## 💾 Data & storage

Tasks, clients, and artifacts save in your browser's **localStorage**. This means:

- ✅ Data persists between sessions on the same browser
- ✅ Works offline
- ⚠️ Data is per-browser — you and your partner each have separate copies for now
- ⚠️ Clearing browser data will erase it — export important info periodically

**To back up your data:** Open the browser console (`Cmd + Option + J`), type `JSON.stringify(localStorage)` and copy the output somewhere safe.

---

## 🎨 Customizing your branding

All colors are CSS variables at the very top of `index.html`. Find this block:

```css
:root {
  --purple: #3d2b8e;         /* main brand purple */
  --purple-dark: #2a1d6e;    /* hover/dark state */
  --purple-deeper: #1e1352;  /* sidebar background */
  --accent: #7c5dfa;         /* buttons and highlights */
}
```

Change those hex values to update the entire app's color scheme instantly.

---

## 🌐 Setting up a custom domain

Your current URL is auto-generated. To use something like `pm.escapewd.com`:

1. In Netlify → **Domain management** → **Add domain**
2. Follow their DNS setup steps (takes ~10 min)
3. Free SSL certificate included automatically

---

## 🤝 Adding real-time team sync (future upgrade)

Currently data is stored locally per browser. To sync between you and your partner in real time, the next step is adding a free database like **Supabase** or **Firebase**. Ask Claude to help wire that up when you're ready — it connects directly to this same HTML file.
