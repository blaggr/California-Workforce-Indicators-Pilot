# Deploy guide — GitHub Pages (5 minutes, no command line)

The fastest path to a public URL.

## 1. Sign in to GitHub

If you don't have an account, create one at https://github.com/signup. Use your UCLA email if you want to apply for GitHub Education benefits later; otherwise any email works.

## 2. Create a new repository

- Click **+ → New repository** in the top right.
- **Repository name:** `workforce-indicators-pilot` (or any short, readable slug — this becomes part of your URL).
- **Description:** optional, e.g. *"California Workforce Indicators Pilot — viability findings, AVAL @ UCLA, May 2026."*
- **Visibility:** **Public**. Required for GitHub Pages on the free tier.
- **Initialize:** leave all the checkboxes unchecked. Click **Create repository**.

## 3. Upload the two files

On the new empty repo page, click **uploading an existing file** (it's a small link near the top). Drag both files from this bundle into the upload zone:

- `index.html`
- `.nojekyll`

(GitHub may hide the `.nojekyll` file in some views because it starts with a dot — that's fine, the file is still uploaded.)

Scroll down, leave the commit message as default, and click **Commit changes**.

## 4. Turn on GitHub Pages

- In the repo, click **Settings** (top right).
- In the left sidebar, click **Pages** (under "Code and automation").
- Under **Build and deployment → Source**, choose **Deploy from a branch**.
- Under **Branch**, choose **main** and **/ (root)**, then click **Save**.

GitHub now builds the site. Refresh the Pages page after 30–60 seconds. You'll see a green box with your live URL:

```
Your site is live at https://YOUR-USERNAME.github.io/workforce-indicators-pilot/
```

## 5. Share the URL

That URL is permanent (as long as the repo stays public). Share it in emails, Slack, decks, Box folders — anyone with a browser can open it.

## Updating the page later

When the report changes, regenerate `index.html` from the AVAL infographic-report skill (or the source v7 HTML). Then:

- In your repo, click on `index.html` → click the pencil icon → upload the new file → commit.
- Pages rebuilds within 60 seconds.

## Optional: custom domain

If you have a domain (e.g., `report.aval.ucla.edu`), GitHub Pages supports custom domains for free. In the same Settings → Pages page, add the domain under **Custom domain**, then add a CNAME record at your DNS provider pointing to `YOUR-USERNAME.github.io`. SSL is automatic.

## Optional: track views (privacy-friendly)

To know how many people opened the report without using Google Analytics, add a one-line snippet from a privacy-respecting analytics provider:

- **Plausible:** $9/month, no tracking cookies, GDPR-compliant. Add their script tag in `<head>`.
- **GoatCounter:** free for non-commercial, no cookies. https://www.goatcounter.com/
- **Umami:** self-hosted or $9/month cloud. https://umami.is/

None of these are installed in the public HTML. If you want one added, regenerate `index.html` with the snippet placed right before `</head>`.

## Alternative platforms (if GitHub feels heavy)

**Cloudflare Pages** — drag-and-drop `index.html` at https://pages.cloudflare.com/. No git required. Auto-generated URL like `aval-workforce.pages.dev`. Faster CDN than GitHub Pages.

**Netlify** — drag-and-drop at https://app.netlify.com/drop. Same flow, URL like `aval-workforce.netlify.app`. Free SSL, free custom domain.

**Both are perfectly fine.** I recommended GitHub Pages above because the `*.github.io/*` URL pattern reads as authoritative-academic to policy audiences. If your audience is more general (foundation funders, CWDA conference attendees, social-share traffic), Netlify or Cloudflare's nicer URLs and faster first-load might be the better fit.
