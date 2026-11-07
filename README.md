# Joshua Rowan — GIS & Remote Sensing Portfolio

A simple, responsive personal portfolio for GitHub Pages. It has four pages, shared styling, and draft text based on your described work. It uses ordinary HTML and CSS. There is no installation or build step.

## Start here

1. Unzip this package.
2. Double-click `index.html` to preview the website in a browser. Navigation and styling also work without a server.
3. Review every page's wording. Add actual map exports, checked findings, your contact links, and any reports you wish to share before treating it as a finished portfolio.
4. Follow the publishing steps below. The site has not been published or connected to your GitHub account.

## Publish using the GitHub website

1. Sign in to https://github.com/ or create a personal account.
2. Choose **New repository**. Name it **YOUR-USERNAME.github.io**, replacing YOUR-USERNAME with your actual GitHub username in lowercase. The name must match your username.
3. Choose **Public** if you use GitHub Free. Turn on **Add README**, then create the repository. All uploaded source files and included reports will be public.
4. In the repository, choose **Add file → Upload files**. Drag the contents of the unzipped folder into the upload area. Upload the files, not the ZIP and not the enclosing folder. Keep the `assets` folder intact. `index.html` must be directly at the top level of the repository.
5. Click **Commit changes**. A commit saves a version of your files.
6. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Choose **main**, then **/(root)**, and save.
7. Allow up to 10 minutes for publication. Return to **Settings → Pages → Visit site**. The address will use your actual username followed by `.github.io`.

If you already use that repository for an existing website, preserve it and use a new project repository instead. These files use relative links and work at a project-site address too. Follow the same branch/root publishing steps.

## What each file does

| File | Purpose |
| --- | --- |
| `index.html` | Homepage, biography, selected projects, skills; optional contact block |
| `gis-work.html` | Georeferencing and GIS experience |
| `remote-sensing.html` | Mont Jacques-Cartier and water mapping project overviews |
| `research-reports.html` | Research interests and project documentation |
| `assets/styles.css` | Colours, fonts, spacing, and responsive layouts |
| `assets/images/` | Your exported maps and photographs |
| `assets/reports/` | Your reviewed PDFs and CV |

## Edit text through GitHub

Open an HTML file in the repository, select the pencil icon, change the words between the tags, then **Commit changes**. For example:

```html
<p>Replace this sentence with your own description.</p>
```

Keep the tags such as `<p>`, `</p>`, and `<h2>` in place. Comments beginning `<!-- EDIT:` identify content to personalize. Updates publish automatically from the selected branch.

## Add a real map

Export a PNG or JPG from QGIS or ArcGIS Pro and upload it to `assets/images/`. Insert this block into the relevant project's HTML, replacing the filename, alternative text, caption, and data credits with accurate details:

```html
<figure>
  <img class="project-image" src="assets/images/YOUR-MAP.png"
       alt="Describe the actual map and the pattern it shows."
       loading="lazy">
  <figcaption>Actual map title. Data sources: add the real credits.</figcaption>
</figure>
```

The example path is a template, not an included file. Use a readable web-sized export and offer a PDF for detailed labels. Each page can use the same layout. No illustrative maps are presented as your results.

## Add a PDF or StoryMap link

After uploading the actual PDF to `assets/reports/`, add a link:

```html
<a class="download" href="assets/reports/YOUR-REPORT.pdf">Download the report (PDF)</a>
```

For an existing StoryMap, add your actual public URL:

```html
<a class="download" href="YOUR-PUBLIC-STORYMAP-URL">Open the interactive StoryMap</a>
```

## Add contact information

An optional contact section is commented out near the bottom of `index.html`. Replace YOUR_EMAIL and YOUR_LINKEDIN_URL with real details, add your CV PDF if desired, then remove the surrounding comment markers. Only include links to files and accounts that actually exist. No contact details have been guessed.

## Change the style

At the top of `assets/styles.css`, `--green` controls the accent colour, `--canvas` the outside background, and `--ink` the main text colour. Headings use Georgia and body text uses the visitor's system font, so the site does not depend on an external font service.

## Before sharing the link

- Review your biography, current program, and descriptions of professional responsibilities.
- Add your strongest actual map and verified project findings. Draft summaries include no invented numerical results.
- Check downloads, labels, and layout on a phone and a computer.
- Open the published site in a private browser window to check that linked web maps and reports are publicly accessible.
- Treat this as a personal/project portfolio. GitHub Pages is not intended as free hosting for running an online business, e-commerce, or a site primarily facilitating commercial transactions. If the site develops into that kind of consulting business website, use appropriate hosting. The same HTML/CSS files can be moved.

## Official instructions

- GitHub Pages quickstart: https://docs.github.com/en/pages/quickstart
- Creating a GitHub Pages site: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- GitHub Pages usage limits: https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
