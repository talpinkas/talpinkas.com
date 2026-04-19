# CLAUDE.md - talpinkas.com

## Project overview

Personal website for Tal Pinkasovich. Static HTML site hosted on GitHub Pages with Cloudflare DNS.

- **Live URL:** https://talpinkas.com
- **Repo:** github.com/talpinkas/talpinkas.com
- **Hosting:** GitHub Pages (free)
- **DNS:** Cloudflare (free plan)
- **Domain registrar:** Cloudflare (~$10/year)
- **Stack:** Single index.html file, vanilla HTML/CSS/JS, no framework, no build step

## Site structure

The entire site is one `index.html` file containing:

1. **Nav** — Tal Pinkasovich | כתיבה | מעבדה | אודות | צור קשר | EN/עב toggle
2. **Hero** — "Tal Pinkasovich / Indoor. Outdoor. Within."
3. **Writing** — List of articles with dates, titles, tags (Defense/JPost), and links to LinkedIn articles or JPost
4. **Lab (מעבדה)** — Projects section with CHOOSY and Pink Ace GTO (descriptions TBD)
5. **About** — Professional background (left column) + Indoor/Outdoor/Within categories (right column)
6. **Contact** — LinkedIn + talpinkas@gmail.com
7. **Footer** — Copyright + talpinkas.com

## Bilingual support

The site is bilingual (Hebrew/English) with a toggle button in the nav. Implementation:

- Default language is Hebrew (RTL)
- Switching to English changes `dir="ltr"`, body class, and updates all elements with `data-he`/`data-en` attributes
- Hero title and Indoor/Outdoor/Within categories stay in English in both languages
- Article titles stay in English in both languages (articles are written in English)
- Nav, section labels, and about text switch between languages

## Design principles

- Minimalist, black and white, no color
- Heavy typography (Space Grotesk for English, Heebo for Hebrew, Space Mono for monospace)
- No emojis, no decorative elements
- Article list is clean rows: date | title | tag
- Lots of whitespace
- Hover effects: article titles turn red, rows shift slightly

## Editorial rules (for any text content)

- No em dashes, no semicolons
- Periods outside quotation marks
- Sentence case headings
- No AI-sounding constructions
- Direct, concise writing

## Published articles (current)

| Date | Title | Tag | Source |
|------|-------|-----|--------|
| 03.2026 | The Paradox Machine: How the AI That Was Banned Won the War | JPost | jpost.com/defense-and-tech/article-890738 |
| 03.2026 | The Paradox Machine: Anthropic, the Pentagon, and the Friction That Matters | Defense | LinkedIn |
| 03.2026 | The American Shahed: Why the Cheapest Drone in the War Is Actually the Most Expensive | Defense | LinkedIn |
| 02.2026 | Code Wins Wars: The Paradigm Shift Reshaping Western Defense | Defense | LinkedIn |
| 02.2026 | The Last Human Safety Catch | Defense | LinkedIn |
| 02.2026 | Your Backyard Is the New Front Line: Calling the Police Won't Help | Defense | LinkedIn |
| 02.2026 | Pricing the Battlefield: What Human Life Costs Defense | Defense | LinkedIn |

## About section content

**Professional Background (English):**
Over a decade in business development, operations, and product management at tech startups. IDF Reservist officer. Experienced in defense technology and national security.

**Professional Background (Hebrew):**
למעלה מעשור בפיתוח עסקי, תפעול וניהול מוצר בסטארטאפים טכנולוגיים. קצין מילואים בצה״ל. ניסיון בטכנולוגיות הגנה וביטחון לאומי.

**Categories:**
- Indoor: Tech. Startups. Defense. EW. Space.
- Outdoor: Ultimate Frisbee. NLH. Nature. Food.
- Within: Family. Stoicism. Life.

## Contact info

- LinkedIn: https://www.linkedin.com/in/talpinkas/
- Email: talpinkas@gmail.com

## Deployment

Any change to `index.html` on the `main` branch auto-deploys to GitHub Pages within ~1 minute.

To update the site:
1. Edit index.html in the repo
2. Commit to main
3. GitHub Pages auto-deploys

## Pending tasks

- [ ] Add descriptions for CHOOSY and Pink Ace GTO in Lab section
- [ ] Add a news/feed page (new feature request)
- [ ] Consider adding a Notes/Short Takes section for LinkedIn posts
- [ ] Translate article titles to Hebrew (decided against — articles are in English)

## Security notes

- Do not include IDF unit name, rank, or specialization details on the public site
- "IDF Reservist officer" is the approved phrasing
- NLH = No Limit Hold'em (poker reference kept as abbreviation intentionally)
