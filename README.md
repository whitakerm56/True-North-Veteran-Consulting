# True North Veteran Consulting — Demo Site

A static, multi-page demo site built for GitHub Pages. No build step, no framework — plain HTML/CSS so it's fast, easy to edit, and easy for Tim to preview immediately.

## Structure
```
/index.html                                   Home
/about.html                                   About Tim
/services.html                                Services
/how-it-works.html                            How It Works
/resources.html                               Resources index
/resources/nexus-letter-sleep-apnea-ptsd.html Sample SEO article
/contact.html                                 Contact / consultation request (demo form, not wired to a backend)
/css/style.css                                Shared stylesheet (design tokens at the top)
/assets/camo-pattern.svg                      Generated four-color digital camo pattern
/assets/favicon.svg
/robots.txt
/sitemap.xml
```

## Deploying to GitHub Pages
1. Create a new repo (e.g. `true-north-site`) and push everything in this folder to the `main` branch, at the repo root.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch," branch `main`, folder `/ (root)`.
4. Save — GitHub will publish at `https://<username>.github.io/true-north-site/`.
5. For a custom domain later (e.g. `truenorthveteranconsulting.com`), add a `CNAME` file at the repo root containing just the domain, and point your domain's DNS to GitHub Pages per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Before this goes live for real (not just as a demo)
- **Placeholder content to replace**: phone number, email, Tim's last name/credentials, and the domain used in canonical URLs, schema markup, `robots.txt`, and `sitemap.xml` (currently `truenorthveteranconsulting.com` as a placeholder).
- **Accreditation language**: every page currently reflects "accreditation pending." Update this the moment that status changes, and have the final claims-support copy reviewed by someone familiar with VA accreditation law (38 U.S.C. § 5904 / 38 CFR Part 14) before this represents a real, live business — several state laws also restrict fees for claims assistance.
- **Contact form**: the intake form is a static demo, not connected to any backend. A production version needs a HIPAA-aware form/storage vendor (with a signed BAA) before it collects any medical records or VA decision letters — see the earlier conversation for why this matters.
- **Real photography**: the "patch" circles are placeholder camo graphics standing in for Tim's photo and provider headshots.

## SEO notes
- Every page has a unique title, meta description, canonical tag, and Open Graph tags.
- Schema.org JSON-LD included: `LocalBusiness` (home), `FAQPage` (How It Works, sample article), `Article` (sample article).
- The sample resources article demonstrates the condition-specific content strategy from the SEO research — this pattern (one article per high-opportunity keyword) is what to replicate for the "Coming Soon" cards on the Resources page.
- `sitemap.xml` and `robots.txt` are ready to submit to Google Search Console once the real domain is live.
