# Xihua (Andy) Xiang — Engineering portfolio

A buildless, static portfolio compatible with GitHub Pages. Edit the HTML and CSS directly; no package installation or build step is required.

## Files

- `index.html`: introduction, project cards, four project stories, about and contact.
- `assets/styles.css`: theme variables, layouts and responsive rules, grouped by section.
- `assets/main.js`: copyright year only. All navigation and content work without JavaScript.
- `assets/favicon.svg`: site favicon.
- `assets/projects/`: supplied project photographs, renders and screenshots.
- Other `assets/*.svg` files are earlier concept illustrations retained on disk and no longer displayed.

## Preview locally

From the repository root, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000`. Stop the server with Ctrl+C.

## Update a case study

Find its article in `index.html`: `dockloop`, `suspension`, `bridge` or `nfc`. Preserve these IDs so project links keep working.

Project stories follow the context, contribution, work and outcome structure naturally in prose. Do not show STAR labels, letter badges or a four-row template to visitors. Keep the project cards to images, names and a “Learn more” link; omit descriptions, category labels and counts.

Replace “To document” and “Not yet documented” only with information you can support. Do not treat a target, estimate or simulation as a measured physical result. Include dates or version numbers where relevant. Keep team achievements distinct from your contribution.

The opening section pairs the name and student role with a subtle drafting grid and a slowly rotating decorative mechanism. The animation stops when reduced motion is requested. Projects, Behind the Designs and About each use one large heading between horizontal rules. Project stories use flowing paragraphs and a simple Photos section for each project.

Project cards are grouped into Featured (DockLoop), Active (DockLoop and NFC cards), and Past (FSAE suspension and bridge). Featured is a curated highlight independent of project status, so DockLoop also appears under Active. Keep card heading IDs unique when showing a project in both groups. Move the existing card into the appropriate `.project-group` when changing groups.

Active/Past describe project status. DockLoop uses supplied project imagery: a connection render, physical prototype photograph and app demo screenshot. FSAE uses the supplied assembly render, detailed render and front view in `assets/projects/fsae/`. The 316 px assembly render stays at its native size in the gallery. The bridge uses supplied photos of the assembled bridge and load test, plus an annotated render in `assets/projects/bridge/`. NFC uses the supplied physical-card photograph and CAD screenshot in `assets/projects/nfc/`. All four projects now show supplied project imagery.

## Add engineering imagery

Create a project folder such as `assets/projects/suspension/` when original images are available. Use descriptive filenames, for example `assembly-cad-v2.webp` or `prototype-test-01.jpg`. Keep paths relative for GitHub Pages compatibility.

Replace the concept image in the relevant `<figure>` and update its `alt`, `width`, `height` and `<figcaption>`. Use the image's real pixel dimensions. Figures preserve the full image, so drawing annotations remain visible. Keep essential information readable in nearby text as well as images.

Add original CAD, drawings or project photographs as figures inside each `.project-gallery`. Caption each item with the design decision or result it supports. Optimise large images before adding them and retain `loading="lazy"` below the hero.

If updating a project card, update its image too. Card images currently have empty alt text because the enclosing link is named by the project title; describe substantive evidence in the case study.

## Content to confirm

- The LinkedIn URL was retained from the original site. Confirm it points to the intended profile.
- DockLoop: a universal connection standard is in development. The app demo uses simulated data, including a key-removal event at a home dock; do not describe this as working sensor integration. Ideation, product design, the entire app demo and roadmap are Andy's contributions. Originally developed for the 2026 Swinburne Student Hackathon, where the team won 1st place overall, as confirmed by the owner. Andy describes a leading role in ideation and product design, development of the entire interactive app demo, and helping shape the roadmap. The supplied render, prototype photo and simulated-data app demo screenshot are in `assets/projects/dockloop/`.
- NFC cards: PLA cards made with dual-nozzle 3D printing for the lettering, with two independently programmable chips linking to user-selected destinations. The physical-card photograph and CAD screenshot are in `assets/projects/nfc/`; add design iterations and tap-testing observations.
- FSAE: wheel hubs and rims designed in SolidWorks, with both simulated and physical load testing on all owned parts for performance and endurance. Supplied renders are in `assets/projects/fsae/`; add test conditions and results.
- Bridge: 860 mm clear span, 372 g mass and a highest tested load of 3,100 N; this is not a stated failure load. The owner reports the best strength-to-weight ratio among the project bridges. Andy contributed research, assembly and testing. Supplied imagery shows the assembled bridge with its initial small-scale model, severe deflection after 3,100 N in the test rig, and an annotated component render.
- All four projects have supplied imagery. No unconfirmed CAD package, manufacturing process or performance check is claimed.

## Before publishing

Check the site at desktop, tablet and phone widths, including 320px. Test every link and keyboard focus, zoom to 200%, and ensure figures and captions remain readable. Check contrast and reduced-motion behaviour. All core content must remain usable with JavaScript disabled.

The existing GitHub Pages hosting arrangement can serve these files directly. No routing service, backend or external font service is needed. Publishing or pushing changes requires the owner's explicit approval.
