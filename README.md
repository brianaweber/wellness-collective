# The WELLness Collective — Client Portal

A personalized, branded client portal system hosted free on GitHub Pages.

---

## How It Works

Each client gets their own page at a unique URL:
```
https://yourusername.github.io/wellness-collective/clients/sarah.html
https://yourusername.github.io/wellness-collective/clients/jessica.html
```

No logins. No accounts. Just a private link.

---

## Adding a New Client

### Step 1 — Copy the template
Duplicate `clients/template.html` and rename it to your client's first name (lowercase):
```
clients/sarah.html
clients/jessica.html
```

### Step 2 — Edit the CLIENT_DATA block
Near the top of the `<script>` section, find `const CLIENT_DATA = { ... }` and update:

| Field | What it is |
|---|---|
| `name` | Client's first name (shows in header) |
| `fullName` | Full name |
| `startDate` | Program start date |
| `goal` | Their main goal (shows on overview) |
| `coach` | Your name |
| `split` | Days per week (3, 4, or 5) |
| `stepGoal` | Daily step target |
| `proteinGoal` | Daily protein target |
| `waterGoal` | Daily water target |
| `weeklyFocus` | Array of 6 weekly focus phrases |

### Step 3 — Add their workouts
Under `"weeks"`, fill in their workout days, exercises, sets, reps, warmup, and cooldown.

### Step 4 — Push to GitHub
```bash
git add .
git commit -m "Add client: Sarah"
git push
```

### Step 5 — Send them their link
```
https://yourusername.github.io/wellness-collective/clients/sarah.html
```

---

## First-Time GitHub Setup

1. Create a free account at [github.com](https://github.com)
2. Create a new repository named `wellness-collective`
3. Upload all files from this folder
4. Go to **Settings → Pages → Source → main branch**
5. Your site will be live at `https://yourusername.github.io/wellness-collective/`

---

## What Clients Can Do
- ✅ View their personalized program and weekly workouts
- ✅ Check off exercises as they complete them
- ✅ Track daily habits (saves automatically in their browser)
- ✅ Fill in weekly check-ins
- ✅ Log progress week by week
- ✅ Works on phone and desktop

---

## File Structure
```
wellness-collective/
├── index.html              ← Home page (just shows the brand)
├── README.md               ← This file
├── clients/
│   ├── template.html       ← Copy this for each new client
│   ├── sarah.html          ← Sarah's portal
│   └── jessica.html        ← Jessica's portal
└── data/
    └── sarah.json          ← (Optional) client data reference
```

---

## Branding
Colors, fonts, and design match The WELLness Collective brand guide:
- **Fonts**: Cormorant Garamond (headings) + Montserrat (body)
- **Colors**: Sage Green, Warm Sand, Cream, Taupe
- **Feel**: Supportive, premium, calming, organized

---

*Built for The WELLness Collective · Coach Briana Weber*
