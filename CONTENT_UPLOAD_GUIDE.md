# Content Upload Guide

This guide explains how to add a new publication or artwork PDF to the academic website.

## What to Send

For each new item, please provide:

- Section: `Publications` or `Artworks`
- Title
- Year
- Authors, for publications
- Venue, journal, conference, exhibition, or short description
- PDF file
- Optional video link
- Optional project link

Example:

```text
Section: Publications
Title: Paper Title
Authors: Yuyang Jiang, Author Two, Author Three
Year: 2026
Venue: Conference Name · Full Paper
PDF: uploaded file
Video: https://example.com/video
```

## File Locations

Publication PDFs and cover images should go here:

```text
assets/publications/
```

Artwork PDFs and cover images should go here:

```text
assets/artworks/
```

Recommended file names use lowercase letters, numbers, and hyphens:

```text
digital-mustard-garden.pdf
digital-mustard-garden-cover.jpg
see-my-sea.pdf
see-my-sea-cover.jpg
```

## PDF Cover Image

When you upload a PDF, Codex can generate a cover image from the first page of the PDF.

The cover image will be used as the representative image in the website item card.

Recommended cover image format:

- `.jpg` or `.png`
- Vertical image
- Around `900 x 1200px`, or any similar portrait ratio

## Website Entry Format

Publication entries use this structure:

```html
<article class="publication-row">
  <img class="publication-image" src="assets/publications/example-cover.jpg" alt="Representative image for Paper Title" width="180" height="240" loading="lazy">
  <div class="publication-copy">
    <h3>Paper Title</h3>
    <p class="publication-authors"><strong>Yuyang Jiang</strong>, Author Two, Author Three</p>
    <p class="publication-year">2026</p>
    <p class="publication-venue">Conference Name · Full Paper</p>
    <div class="publication-actions">
      <a class="publication-button" href="assets/publications/example.pdf">PDF</a>
      <a class="publication-button" href="https://example.com/video" target="_blank" rel="noreferrer">Video</a>
    </div>
  </div>
</article>
```

Artwork entries use this structure:

```html
<article class="artwork-row">
  <img class="artwork-image" src="assets/artworks/example-cover.jpg" alt="Representative image for Artwork Title" width="180" height="240" loading="lazy">
  <div class="artwork-copy">
    <h3>Artwork Title</h3>
    <p class="artwork-year">2026</p>
    <p class="artwork-details">Medium · Exhibition or project description</p>
    <div class="artwork-actions">
      <a class="artwork-button" href="assets/artworks/example.pdf">PDF</a>
      <a class="artwork-button" href="https://example.com/project" target="_blank" rel="noreferrer">Project</a>
      <a class="artwork-button" href="https://example.com/video" target="_blank" rel="noreferrer">Video</a>
    </div>
  </div>
</article>
```

## Publishing Steps

After the files and website entry are updated:

1. Preview the website locally.
2. Check that the cover image loads.
3. Check that the PDF button opens the correct PDF.
4. Commit the change.
5. Push the repository to GitHub.

GitHub Pages will update the live website after the push.
