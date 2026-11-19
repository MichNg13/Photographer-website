# Alice Huang, Photographer

One-page portfolio site for a freelance wedding and portrait photographer: hero with a contact button, a six-image portfolio grid, a short about section, and an email contact block.

It is a static site with no build step.

## Files

- `index.html`: the whole site, with its styles inline. This is what gets deployed.
- `images/`: portfolio photos, referenced from `index.html`.
- `vercel.json`: Vercel settings (static site, long cache for images).
- `project/`: the original Claude Design source (`Main.dc.html`, `canvas.json`). Not used by the deployed site.

## Run locally

```sh
npx serve .
```

Or open `index.html` directly in a browser.

## Deploy to Vercel

1. In Vercel, choose **Add New > Project** and import this repository.
2. Leave Framework Preset as **Other**, and leave Build Command and Output Directory empty.
3. Click **Deploy**.

Or from the command line: `npx vercel --prod`.

## Editing

- Add a photo: put the file in `images/`, then replace a "Photo N" placeholder `<div>` in `index.html` with an `<img src="images/your-file.jpg" alt="...">`, copying the one for the first photo.
- Change the email: replace `hello@example.com` (it appears twice in the contact section).
- Change the about text: edit the two paragraphs under "About".
