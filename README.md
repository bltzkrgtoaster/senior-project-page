# Victor Bellmore | Custom Costuming (Senior Project Portfolio)

A static site: no build step, no dependencies. `index.html` is the whole site.

## Deploy to Cloudflare Pages

### Option A: Direct upload (fastest)
1. Log in at https://dash.cloudflare.com and go to **Workers & Pages**.
2. Click **Create**, then the **Pages** tab, then **Upload assets**.
3. Name the project (for example `victor-costuming`). This becomes `victor-costuming.pages.dev`.
4. Upload the `site` folder (or the unzipped contents) so `index.html` is at the top level.
5. Click **Deploy**.

To update later, open the project, choose **Create new deployment**, and upload the changed files.

### Option B: Git (auto-deploys on every push)
1. Put this folder in a GitHub repository.
2. In **Workers & Pages**, choose **Create**, then **Pages**, then **Connect to Git**, and pick the repo.
3. Framework preset: **None**. Build command: leave empty. Build output directory: `/`.
4. Click **Save and Deploy**.

## Notes
- Page navigation uses URL hashes (like `/#mentor`), so no redirect rules are needed.
- Fonts load from Google Fonts and fall back to system fonts if blocked.
