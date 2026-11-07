# EarnWithProof — Static Site Scaffold

Plain HTML/CSS website for **EarnWithProof**: honest, proof-based guides to earning online (AI tools & automation, freelancing, digital products, KDP publishing, SEO & blogging, finance basics), written by Tanvir Ahmed from first-hand experience. No build step, no framework — ready to host free on GitHub Pages, exactly like the author's other sites.

> Brand note: the site was renamed from "ToolNOva AI" to **EarnWithProof** on 2026-11-07 because "ToolNova" is already owned by several established tool sites. The folder keeps its original name (`toolnova-site/`); only the branding/copy changed. Positioning: every guide shows the proof — real screenshots, fee receipts, timelines — instead of guru income claims.

## Files

| File | What it is |
|---|---|
| `index.html` | Homepage: hero, 7 category cards, Latest articles list (empty state), About teaser, footer with disclaimer |
| `about.html` | About the site + "About the author" (Tanvir Ahmed) |
| `contact.html` | Contact via the EarnWithProof blog/social profiles (no email address is published — no verified domain email exists yet) |
| `privacy.html` | Privacy Policy (short placeholder version) |
| `terms.html` | Terms of Use (educational content, no earnings guarantee) |
| `make-money-online.html` | Category page: Make Money Online |
| `ai-tools.html` | Category page: AI Tools & Automation |
| `freelancing.html` | Category page: Freelancing |
| `ecommerce.html` | Category page: E-Commerce & Digital Products |
| `kdp-publishing.html` | Category page: KDP & Publishing |
| `seo-blogging.html` | Category page: SEO & Blogging |
| `finance-basics.html` | Category page: Finance Basics |
| `article-template.html` | Reusable article page — copy this for every new article |
| `styles.css` | The one shared stylesheet for the whole site (light theme, responsive, card grid) |
| `sitemap.xml` | Sitemap skeleton: homepage, 7 category pages, 4 info pages. Article URLs get added as articles are written |
| `robots.txt` | Allows all crawlers; points to the sitemap |

## How to add an article

1. **Copy** `article-template.html` and rename the copy to the article slug, e.g. `first-fiverr-order-timeline.html`.
2. **Fill in** the title, meta description, breadcrumb (category page + name), H1, lede, Key Takeaways box and body sections. Delete the instruction comments at the top. Keep the author box. Keep the finance disclaimer block on all Finance Basics posts (and any post discussing fees, taxes or earnings figures).
3. **Link it in 3 places:**
   - Its **category page** — replace/extend the `.article-list` area with an `.article-item` block (remove the `.empty-state` div once the first article exists in that category).
   - The **homepage** `index.html` "Latest articles" list — add an `.article-item` block, newest first (remove the `.empty-state` div once the first article exists).
   - **`sitemap.xml`** — add a `<url>` block for the new article.
4. **Related articles:** add 2–4 links in the article's own "Related articles" area, and link back to it from related older articles where relevant.

## Before launch (GitHub Pages)

1. Create the GitHub repo and push this folder's contents (repo creation is done by the site owner — this scaffold does not publish anything by itself).
2. Replace the placeholder `https://your-site-url.example` in **sitemap.xml** and **robots.txt** with the real live URL.
3. Add the site to Google Search Console and submit `sitemap.xml`.
4. Publish articles in small batches (a few per day) rather than all at once, and check Search Console after 3–4 weeks to see which topics Google rewards before scaling up.

## House rules for content

- English only; target readers in English-speaking countries (US/UK/EU).
- No income promises, no "get rich quick" language, no invented earnings.
- Every guide needs a first-hand element: a screenshot, fee receipt, real timeline or documented mistake.
- Finance Basics = educational explainers with disclaimers only. No stock/crypto/forex trading advice.
