# Tiffany's Kitchen & Bar — Project Tracker

**Client:** Tiffany's Kitchen & Bar (restaurant, catering, private events)
**GitHub:** `ffgroup-8/tiffanys-kitchen-bar` → https://github.com/ffgroup-8/tiffanys-kitchen-bar
**Local:** `~/Desktop/Git Repo/Tiffany's/index.html`
**Live:** https://ffgroup-8.github.io/tiffanys-kitchen-bar/

---

## Master Rules

Follow all rules in `../_Project Tracker Master/CLAUDE.md`. That file is the source of truth for:
- Box hierarchy (`seo-box` → `content-created-box` as siblings)
- CSS patterns (green seo-box, blue content-created-box, dark mode)
- Status pill system (6 categories)
- SEO standards
- Push-automatically rule
- Content writing standard (actual copy, not design annotations)

**Pipeline:** If you add a new pattern here that isn't in Master, also apply it to `../_Project Tracker Master/index.html` and commit both.

---

## Current Progress

| Category        | Progress |
|-----------------|----------|
| Design          | (check tracker) |
| Dev             | (check tracker) |
| SEO             | (check tracker) |
| Content Input   | (check tracker) |
| Sanity Dev      | (check tracker) |
| Content Created | 0% (0/13 pages complete) |

---

## Pages (13 content pages)

| # | Page | Slug | Content Created |
|---|------|------|-----------------|
| 1 | 🏠 Home | `/` | ⬜ needed |
| 2 | 🍽️ Menus & Location | `/menus` | ⬜ needed |
| 3 | 🥡 Catering | `/catering` | ⬜ needed |
| 4 | 🎉 Private Parties | `/private-parties` | ⬜ needed |
| 5 | 📖 History / About | `/about` | ⬜ needed |
| 6 | ⭐ Rewards | `/rewards` | ⬜ needed |
| 7 | 🎁 Gift Cards | `/gift-cards` | ✅ done (used as reference model) |
| 8 | 🤝 Donations | `/donations` | ⬜ needed |
| 9 | 💼 Careers | `/careers` | ⬜ needed |
| 10 | 🎟️ Events & Offers | `/events` | ⬜ needed |
| 11 | 📬 Contact | `/contact` | ⬜ needed |
| — | Knowledge Base sections | — | n/a |

---

## Content Notes

- Gift Cards page was the **reference model** for how `content-created-box` content should look — actual copy (headlines, body, CTAs), not design annotations
- Brand voice: Warm, welcoming, community-focused. Family restaurant energy.

---

## Content Module Template

```html
<p><strong>📌 Module 1 — Hero</strong></p>
<ul>
  <li><strong>Headline:</strong> ...</li>
  <li><strong>Subheadline:</strong> ...</li>
  <li><strong>CTA:</strong> ...</li>
</ul>
```

After adding content for a page:
1. Mark Content Created pill `completed` in both nav-item AND sitemap node
2. Recalculate `data-target` on Content Created progress bar: `(N / 13 * 100).toFixed(0)%`
3. Commit and push automatically
