# KRH proposal pack generation: interactive architecture

An interactive diagram of the proposal generation design for KRH: Salesforce, MuleSoft and the Claude API.

- **Two flows:** Generate pack, and Edit a section
- **Two explanation styles:** Technical, and Business (plain language)
- Click any block for details, or use **Walk through the flow** (arrow keys also work)

Everything is in a single self-contained `index.html`. The only external request is the Rubik font from Google Fonts, which falls back to the system font if it can't load.

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `krh-proposal-flow`.
2. Upload `index.html`, `README.md` and `.nojekyll` to the root of the `main` branch. On the web, use **Add file → Upload files** and drag them in, or from a terminal:
   ```bash
   git init
   git add .
   git commit -m "KRH proposal flow diagram"
   git branch -M main
   git remote add origin https://github.com/<your-username>/krh-proposal-flow.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
5. After a minute or two the site is live at `https://<your-username>.github.io/krh-proposal-flow/`.

To update the diagram later, replace `index.html` and commit. Pages redeploys automatically.

## Before sharing

GitHub Pages sites are publicly accessible on standard plans, even when the repository is private. This page names the client (KRH) and describes the solution design, and uses WarpDrive brand assets. Confirm that's acceptable before sharing the link outside the team.

Cost figures in the diagram are estimates at Claude Opus 5.5 list prices as of 13 Oct 2026.
