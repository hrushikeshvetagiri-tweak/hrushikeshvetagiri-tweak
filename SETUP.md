# GitHub profile README — setup guide

**For:** Vetagiri Hrushikesh · `@hrushikeshvetagiri-tweak`

This folder contains everything for your personal GitHub profile page — the README that appears at [github.com/hrushikeshvetagiri-tweak](https://github.com/hrushikeshvetagiri-tweak).

---

## What you get

| File | Purpose |
|------|---------|
| `README.md` | **Recommended** — native GitHub styling, Mermaid, collapsible sections, stats |
| `README.minimal.md` | Shorter variant — logo, one diagram, stats |
| `assets/logo.png` | Tweak product logo (PNG) |
| `assets/tweak-banner.svg` | Unused source art — README uses GitHub's own background, no banner |

---

## Part 1 — Create the repo on GitHub (UI, step by step)

### Step 1: Sign in

1. Open [github.com](https://github.com) and sign in as **hrushikeshvetagiri-tweak**.

### Step 2: New repository

1. Click the **+** icon (top-right) → **New repository**.
2. Fill in exactly:

   | Field | Value |
   |-------|--------|
   | **Owner** | `hrushikeshvetagiri-tweak` |
   | **Repository name** | `hrushikeshvetagiri-tweak` ← must match username exactly |
   | **Description** | `GitHub profile — Founder of Tweak (tweak.page)` |
   | **Public** | ✅ selected |
   | **Add a README file** | ✅ check this (easier first push) |
   | **Add .gitignore** | None |
   | **Choose a license** | None |

3. Click **Create repository**.

> **Why the name must match:** GitHub only renders `README.md` on your profile when the repo name equals your username.

### Step 3: Confirm it works (empty README)

1. Go to [github.com/hrushikeshvetagiri-tweak](https://github.com/hrushikeshvetagiri-tweak).
2. You should already see the default README from that repo on your profile.

---

## Part 2 — Upload files

### Option A — GitHub web UI (no terminal)

1. Open `https://github.com/hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak`.
2. Click **Add file** → **Upload files**.
3. Drag in from this folder:
   - `assets/tweak-banner.svg` (create `assets/` if prompted)
4. Commit: `Add Tweak banner asset`.

5. Open `README.md` → click **pencil (Edit)**.
6. Delete all content.
7. Paste the full contents of **`README.md`** from this folder (or `README.minimal.md` if you prefer minimal).
8. Commit: `Add profile README`.

9. Refresh [github.com/hrushikeshvetagiri-tweak](https://github.com/hrushikeshvetagiri-tweak) — banner + bio should appear within ~30 seconds.

### Option B — Terminal (recommended if you use git daily)

```bash
# Clone the profile repo
git clone https://github.com/hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak.git
cd hrushikeshvetagiri-tweak

# Copy files from tweak.page workspace (adjust path if needed)
mkdir -p assets
cp /Users/hrushi.tweak/Tweak/tweak.dev/tweak.page/profile-repo/assets/tweak-banner.svg assets/
cp /Users/hrushi.tweak/Tweak/tweak.dev/tweak.page/profile-repo/README.md README.md

git add assets/tweak-banner.svg README.md
git commit -m "Add profile README with Tweak banner and stats"
git push origin main
```

**Minimal variant instead:**

```bash
cp /Users/hrushi.tweak/Tweak/tweak.dev/tweak.page/profile-repo/README.minimal.md README.md
git add README.md && git commit -m "Use minimal profile README" && git push
```

---

## Part 3 — Pin repos on your profile

1. Go to [github.com/hrushikeshvetagiri-tweak](https://github.com/hrushikeshvetagiri-tweak).
2. Click **Customize your pins** (or **Pinned** → **Customize your pins**).
3. Pin up to 6 repos — e.g. `tweak.page` when public, `hrushikeshvetagiri-tweak`, MCP-related repos.
4. Save.

---

## Part 4 — Profile settings (optional polish)

1. **Profile photo:** [github.com/settings/profile](https://github.com/settings/profile) → upload photo.
2. **Bio:** e.g. `Founder @ Tweak — live website review on the real DOM · tweak.page`
3. **Website:** `https://tweak.page`
4. **Social:** add LinkedIn / X when ready.

---

## Part 5 — Stats cards troubleshooting

The README uses these services (free, no API key):

| Card | URL |
|------|-----|
| GitHub stats | `github-readme-stats.vercel.app` |
| Streak | `github-readme-streak-stats.demolab.com` |
| Typing line | `readme-typing-svg.demolab.com` |

**If cards show “user not found” or empty:**

- Profile must be **Public** (Settings → Profile → untick “Make profile private”).
- New accounts need at least **one public commit** for language/stats to populate.
- Wait 5–10 minutes after first push — caches refresh slowly.

**If stats look broken:**

- Cards use `theme=github` / `theme=default` so they match GitHub's native light/dark page — no custom background colors in the README.
- If images show as links, wait a few minutes or hard-refresh the profile page.

---

## Part 6 — Choose your variant

| | Dark (full) | Minimal |
|---|-------------|---------|
| **File** | `README.md` | `README.minimal.md` |
| **Banner** | ✅ | ✅ |
| **Stats + streak** | ✅ both + top langs | ✅ stats + streak only |
| **Product detail** | Full tables + stack | One paragraph |
| **Best for** | Founder showcase | Clean, understated |

Switch anytime: replace root `README.md` content and push.

---

## Part 7 — Keep it updated

Every few months, edit **Currently focused on** (full README) or the one-liner (minimal).

When Tweak launches new surfaces (billing, integrations, PH), add a badge or link — keep the profile aligned with [tweak.page](https://tweak.page).

---

## Quick checklist

- [ ] Repo `hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak` exists and is **public**
- [ ] `assets/tweak-banner.svg` uploaded
- [ ] `README.md` pasted (dark or minimal)
- [ ] Profile page shows banner at [github.com/hrushikeshvetagiri-tweak](https://github.com/hrushikeshvetagiri-tweak)
- [ ] Stats cards loading (may take a few minutes)
- [ ] Bio + website set in GitHub settings
- [ ] Product repo pinned

Done — your profile acts as a mini landing page for you and Tweak.
