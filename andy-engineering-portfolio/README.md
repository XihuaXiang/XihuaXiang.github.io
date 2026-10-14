# Xihua (Andy) Xiang — Engineering Portfolio

A ready-to-publish static engineering portfolio with four project case studies. No Node, React, frameworks, build tools, CMS or hosting subscription required.

**Built with:** HTML, CSS, a few SVG placeholder illustrations and a tiny JavaScript file. Designed for **GitHub Pages**.

## Publish on GitHub Pages (browser method)

1. Sign in at https://github.com and create a **public** repository with the exact name `YOUR-GITHUB-USERNAME.github.io` (replace both parts with your username). A README is fine.
2. Unzip the downloaded archive. Open the folder called `andy-engineering-portfolio`.
3. In the new GitHub repository, select **Add file -> Upload files**. Drag **`index.html` and the entire `assets` folder** into the upload area. (You can also include `.nojekyll`, but it is not essential for this site.) Ensure `index.html` is at the **root** of the repository and the files keep their `assets/` paths. If folder uploading does not work in your browser, use the GitHub Desktop method below instead.
4. Click **Commit changes**.
5. Open **Settings -> Pages**. Under **Build and deployment**, choose **Deploy from a branch**; set the branch to **main** and folder to **/(root)**; click **Save**.
6. When GitHub reports deployment, visit `https://YOUR-GITHUB-USERNAME.github.io/`. It can take up to 10 minutes for the first publication.

Official GitHub Docs: https://docs.github.com/en/pages/quickstart

**Important:** An ordinary repository such as `engineering-portfolio` is also supported, but its URL will be `https://YOUR-GITHUB-USERNAME.github.io/engineering-portfolio/`. For your personal home page use the special repo name instead.

## Publish with GitHub Desktop (recommended for ongoing updates)

1. Create the `YOUR-GITHUB-USERNAME.github.io` repository with a README on GitHub.
2. Install GitHub Desktop: https://desktop.github.com/ and sign into your account.
3. Use **File -> Clone repository** to clone your new repo to a folder on your Mac.
4. Copy all files inside this starter folder into that local repository folder. Keep `index.html` at the root.
5. In GitHub Desktop, add a commit message (e.g. `Add engineering portfolio`) and click **Commit to main**, then **Push origin**.
6. Enable **Settings -> Pages -> Deploy from a branch -> main -> /(root)**.
7. Every time you make updates, commit and push them again. GitHub Pages deploys your changes automatically.

## Preview locally

Double-click `index.html`, or run this command from the portfolio directory:

```sh
python3 -m http.server 8000
```

Visit http://localhost:8000 in your browser. Stop the server with Ctrl-C.

## Content to personalise **before sending to employers**

The provided graphics are clearly identified as illustrations, **not** real project CAD, build photos, or demonstrated designs. Project descriptions currently contain deliberately marked `To complete:` notes. Replace them with accurate details before sharing professionally.

### Fast edits

- **Name, study, introduction and LinkedIn:** edit `index.html`; search for `Xihua (Andy) Xiang` and `https://www.linkedin.com/in/xihua-xiang`.
- **Project summaries:** edit the relevant cards in `index.html` (search for `DockLoop`, `Suspension system`, `Bridge design`, or `NFC networking cards`).
- **Longer case studies:** search for `<article` in `index.html` and edit the `<p>` text for your project.
- **Colour palette / typography:** edit the variables at the very top of `assets/styles.css`.
- **Replace illustrations:** copy your own optimised JPG/WebP images into `assets/`, then change the corresponding `<img src="assets/...svg">` paths in `index.html`. Include clear `alt` descriptions and give credit for material that isn't yours.
- **Email and CV:** only add your real address and PDF once you're comfortable making them public. E.g., put `resume.pdf` at the root and link to it with `<a href="resume.pdf">View CV</a>`.
- **Add measurement data:** for the suspension and bridge projects, only include figures supported by coursework, calculations, or test records.

### Suggested evidence for each project

| Project | Useful source material |
|---|---|
| DockLoop | Personal contribution, prototype/CAD, working demo screens, problem, next technical steps, hackathon result |
| Suspension | Original brief, mechanism type, CAD views, loads, calculations, design decisions, evaluation |
| Bridge | Requirements, materials, design sketches, physical construction, predicted and actual performance if measured |
| NFC cards | Photos of iterations, 3D CAD and print setup, NFC tag integration, functional demonstration |

Consider permissions, team consent and IP before publishing detailed DockLoop internals or any university/team work that is not solely yours.

## Folder structure

```
index.html
.nojekyll
.gitignore
README.md
assets/
  styles.css
  main.js
  favicon.svg
  dockloop.svg
  suspension.svg
  bridge.svg
  nfc.svg
```

## Optional: custom domain later

Start with the free `.github.io` URL. When you buy a domain, GitHub Pages supports connecting it through **Settings -> Pages -> Custom domain**, with DNS configuration at the domain provider. Follow: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Site maintenance and privacy

GitHub Pages publishes the site publicly. On GitHub Free, the hosting repository needs to be public. Don't commit keys, private files, unpublished IP details or personal contact information you don't want indexed on the web.

This starter includes no analytics, no tracking pixels, no cookies and no external JavaScript libraries.
