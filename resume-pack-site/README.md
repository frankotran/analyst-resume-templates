# Resume Pack

A $0-budget digital product store: a GitHub Pages landing page selling ATS-friendly resume templates for all job seekers.

**Live site:** https://frankotran.github.io/analyst-resume-templates/

## What's here

- `index.html` — landing page (pricing, previews, FAQ)
- `templates/modern.html` — "Modern Professional" resume template
- `templates/classic-ats.html` — "Classic ATS" resume template
- `templates/compact.html` — "Compact" one-pager template
- `templates/cover-letter.html` — cover letter template with prompts
- `guide.html` — Metric Bullet Formula + 40 examples + ATS checklist (bonus)
- `download.html` — post-purchase delivery page

## Setup (2 steps, ~15 min, $0)

### 1. Enable GitHub Pages
1. Go to this repo → **Settings** → **Pages**
2. Under "Build and deployment", set **Source** to **Deploy from a branch**
3. Set branch to **main**, folder to **/(root)**, click **Save**
4. Wait ~1 minute. Site goes live at https://frankotran.github.io/analyst-resume-templates/

### 2. Connect checkout (Stripe Payment Links — free)
1. Create a free account at https://stripe.com (no monthly fee; Stripe takes 2.9% + $0.30 per sale)
2. Dashboard → **Payment Links** → **Create payment link**
   - Product: "Resume Pack", price **$24** one-time
   - Under "After payment" → redirect customers to: `https://frankotran.github.io/analyst-resume-templates/download.html`
3. Copy the payment link URL, then in `index.html` find `const STRIPE_URL = "";` and paste your link between the quotes
4. Commit the change — checkout is live

### Money math
$24/sale − Stripe fee (~$1.00) = **~$23.00 net per sale**. 10 sales/month ≈ $230/mo for a site that costs $0 to run.

## Upgrade paths (later, still cheap)
- **Gumroad** (free to start, 10% fee) instead of Stripe if you want built-in delivery + license keys
- **Custom domain** (~$12/yr) for credibility
- **Email list** (Buttondown free tier) to capture visitors who don't buy today
