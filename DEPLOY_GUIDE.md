# GigProfitCalc — Deployment & Upgrade Guide
## Created by: Dilshan Nayanajith | nayanajithilangasinghe2002@gmail.com

---

## 📁 Files Delivered

| File | Purpose |
|------|---------|
| `index.html` | Complete upgraded single-page app (all tools + blog) |
| `404.html` | GitHub Pages SPA routing fix |
| `DEPLOY_GUIDE.md` | This file |

---

## ✅ What Was Fixed & Upgraded

### Author & Trust
- [x] Author updated to **Dilshan Nayanajith** everywhere
- [x] Email `nayanajithilangasinghe2002@gmail.com` visible in footer, contact, about, legal pages
- [x] Full author bio section on About page and in every article
- [x] Schema.org `Person` structured data for author

### Fake Claims Removed
- [x] Removed "50K+ Users Helped" — replaced with real tool stats (9 tools, 7 currencies, 100% free, 0% data stored)
- [x] Removed Sri Lanka default currency — USD is now the default
- [x] Removed Sri Lanka-specific keywords and FAQ content
- [x] All income figures clearly labeled as estimates with disclaimers

### SEO
- [x] Title tag optimized for global audience
- [x] Meta description updated (no fake user count)
- [x] Keywords cleaned (no Sri Lanka-only terms)
- [x] Schema.org: WebApplication, Person, FAQPage, BreadcrumbList
- [x] Open Graph + Twitter Card meta tags
- [x] Canonical URL
- [x] Proper heading hierarchy (H1 → H2 → H3)
- [x] aria-label and role attributes added throughout
- [x] Internal linking between tools and articles

### Legal Pages (Full Content)
- [x] **Privacy Policy** — GDPR compliant, full content, AdSense disclosure, affiliate disclosure
- [x] **Terms & Conditions** — Full terms, no income guarantees clause, affiliate disclosure
- [x] **Disclaimer** — Income estimates, tax disclaimer, not financial advice
- [x] **Contact Page** — Real email visible, Formspree integration, form validation

### Blog (5 Full Articles — 1000+ words each)
1. ✅ "How to Start Freelancing in 2026 (Complete Beginner Guide)"
2. ✅ "Top 10 Online Income Ideas That Actually Work in 2026"
3. ✅ "Fiverr vs Upwork: Which Platform Is Better?"
4. ✅ "How Much Can You Really Earn Working Online? Honest Numbers"
5. ✅ "Best Skills to Learn to Make Money Online in 2026"

Each article:
- 1000+ words
- SEO headings (H2, H3)
- Lists and callout boxes
- Author attribution (Dilshan Nayanajith)
- Internal links to relevant calculator tools
- No fake income promises

### Technical Fixes
- [x] Default currency changed from LKR to USD
- [x] Mobile hamburger menu accessibility (aria-expanded)
- [x] Contact form with real Formspree integration + validation
- [x] Hash-based routing improved (handles article sub-routes)
- [x] PopState event listener for browser back/forward
- [x] Disclaimer page added and linked in footer
- [x] Footer includes Disclaimer link
- [x] `404.html` for GitHub Pages SPA fix
- [x] All ad slots have `aria-label="Advertisement"` for accessibility

### AdSense Readiness
- [x] Fake user count removed
- [x] Real disclaimers on every calculator
- [x] 800–1500+ words of content on every important page
- [x] Clear navigation structure
- [x] Privacy Policy mentions AdSense cookies
- [x] Ad slots placed appropriately (not excessive)
- [x] Legal pages all present and complete
- [x] Contact information clearly visible

---

## 🚀 Deployment Steps

### GitHub Pages
1. Create a repository on GitHub (e.g., `gigprofitcalc`)
2. Upload `index.html` and `404.html` to the repository root
3. Go to Settings → Pages → Source: Deploy from Branch → `main` branch → `/ (root)`
4. Your site will be live at `https://yourusername.github.io/gigprofitcalc/`

### Custom Domain (gigprofitcalc.com)
1. Buy the domain from Namecheap, GoDaddy, or Cloudflare
2. In GitHub Pages settings, add your custom domain
3. Create a `CNAME` file in the repo root with content: `gigprofitcalc.com`
4. Point your domain's DNS to GitHub Pages IPs:
   - A records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - CNAME: yourusername.github.io

---

## 📧 Formspree Setup (Contact Form)
1. Go to https://formspree.io and create a free account
2. Create a new form — it gives you a Form ID like `xpzgwkjd`
3. In `index.html`, find: `const FORMSPREE_ENDPOINT = 'https://formspree.io/f/YOUR_FORM_ID';`
4. Replace `YOUR_FORM_ID` with your actual Form ID
5. Free plan: 50 submissions/month. Paid plan: unlimited

---

## 💰 Google AdSense Setup
1. Apply at https://adsense.google.com
2. Add your website URL
3. Paste the AdSense verification code before `</head>` in index.html
4. Wait for approval (typically 1–14 days for new sites with content)
5. Once approved, replace `<!-- AdSense -->` comments in ad slots with actual AdSense code:
   ```html
   <ins class="adsbygoogle"
        style="display:block"
        data-ad-client="ca-pub-XXXXXXXXXX"
        data-ad-slot="XXXXXXXXXX"
        data-ad-format="auto"
        data-full-width-responsive="true"></ins>
   <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
   ```

### AdSense Approval Checklist
- [x] Privacy Policy page present ✅
- [x] Terms & Conditions present ✅
- [x] Disclaimer present ✅
- [x] Contact page with real email ✅
- [x] About page with real author information ✅
- [x] Original content (5 blog articles, 1000+ words each) ✅
- [x] No fake user statistics ✅
- [x] Working navigation ✅
- [x] Mobile responsive ✅
- [x] HTTPS (GitHub Pages provides this automatically) ✅

---

## 🔧 Future Improvements (Optional)
- Add Google Analytics 4 tracking code
- Create OG image (1200×630px) for social sharing
- Add a sitemap.xml for better Google indexing
- Consider adding more blog articles (target: 10+ articles before AdSense application)
- Add JSON-LD BreadcrumbList for each article page

---

## 📬 Contact
**Dilshan Nayanajith**
nayanajithilangasinghe2002@gmail.com
