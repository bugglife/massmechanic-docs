# MassMechanic Static Documentation

Customer-focused static documentation for MassMechanic - designed to be LLM-crawlable without revealing competitive intelligence or operational details.

## What's Included

- **docs/** - Customer-facing static documentation
  - `index.html` - Main documentation landing page
  - `how-it-works.html` - Simple customer journey explanation
  - `service-areas.html` - Geographic coverage information
  - `for-mechanics.html` - Brief info about exclusive network
  - `faq.html` - Customer-focused frequently asked questions

- **llms.txt** - LLM-crawlable summary (no operational details)

## Philosophy

These docs are designed to:
- **Focus on car owners** (primary audience)
- **Protect competitive intelligence** (no scoring algorithms, routing logic, or mechanic pricing)
- **Position as exclusive network** (invitation-only, not open signup)
- **Stay LLM-crawlable** (but without giving away the secret sauce)

## What's NOT Included

Intentionally excluded to protect competitive advantages:
- Lead scoring algorithms and point values
- SMS routing mechanics and territory mapping
- Mechanic subscription pricing or pay-per-lead amounts
- Detailed operational workflows
- Backend technical implementation

## Deploy to GitHub Pages

### Option 1: Use Your Existing Repo

If you already have a MassMechanic docs repo:

1. **Replace the existing docs:**
   - Delete old docs folder
   - Upload new docs folder
   - Replace llms.txt
   - Commit changes

2. **Files should be at:**
   - `https://yourusername.github.io/massmechanic-docs/docs/`
   - `https://yourusername.github.io/massmechanic-docs/llms.txt`

### Option 2: Create New Repo

1. **Create repo** called `massmechanic-docs`
2. **Upload files:**
   - Upload entire `docs/` folder
   - Upload `llms.txt`
   - Commit
3. **Enable Pages:**
   - Settings → Pages
   - Deploy from branch: `main`, folder: `/ (root)`
   - Save

### Custom Domain Setup

If using `docs.massmechanic.com`:

1. **In GitHub repo:**
   - Settings → Pages → Custom domain
   - Enter: `docs.massmechanic.com`
   
2. **In DNS (GoDaddy, etc.):**
   - Add CNAME record
   - Name: `docs`
   - Value: `bugglife.github.io`
   
3. **Wait for SSL:**
   - 30-60 minutes for certificate
   - Enable "Enforce HTTPS" when available

## Link from Main Site

Update your main MassMechanic app:

1. **Add nav link:**
   ```jsx
   <a href="https://docs.massmechanic.com">How It Works</a>
   ```

2. **Create llms.txt at root of massmechanic.com:**
   ```
   # MassMechanic
   
   > For documentation, visit https://docs.massmechanic.com
   
   - Documentation: https://docs.massmechanic.com/
   - How It Works: https://docs.massmechanic.com/how-it-works.html
   - Service Areas: https://docs.massmechanic.com/service-areas.html
   - FAQ: https://docs.massmechanic.com/faq.html
   ```

## Updating Content

When you need to update the docs:

1. Edit HTML files locally
2. Commit and push (or re-upload via GitHub)
3. Changes go live in 1-2 minutes

## Questions?

- GitHub Pages docs: https://docs.github.com/pages
- Contact: support@massmechanic.com
