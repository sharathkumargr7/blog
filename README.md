# sharath.press

A responsive, no-build static blog starter for `sharath.press`. It includes a searchable and filterable journal, article reading dialogs, a custom domain marker, and an automatic GitHub Pages workflow.

## Publish with GitHub Pages

1. Create a repository under `sharathkumargr7` and add these files to its `main` branch.
2. In **Settings → Pages**, set the publishing source to **GitHub Actions**.
3. In **Settings → Pages → Custom domain**, enter `sharath.press` and save. The `CNAME` file alone does not configure this setting.
4. At the DNS provider for the domain, point the apex (`@`) to GitHub Pages using these A records:

   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`

   Optionally add the corresponding IPv6 AAAA records listed in [GitHub's custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site). To use `www.sharath.press` too, add a `CNAME` record for `www` pointing to `sharathkumargr7.github.io` and configure that hostname in Pages.

The workflow deploys on every push to `main`. After DNS propagates, enable **Enforce HTTPS** in Pages settings when GitHub makes it available.

## Editing

The page is a single `index.html` with its styles and interactions inline. Search and topic filters work locally; article cards open their full text in an accessible dialog. The four included notes are starter copy and can be replaced or removed before publishing.

