# Cover Replacement Guide

This guide explains how to replace the representative cover image for a publication or artwork.

## What to Upload

Please upload a `.jpg`, `.jpeg`, or `.png` image and tell Codex which item it belongs to.

Use this format:

```text
Section: Publications / Artworks
Item title:
New cover image: uploaded file
```

Example:

```text
Section: Publications
Item title: Generative Multi-Sensory Meditation
New cover image: uploaded jpg
```

## Recommended Image Format

The website uses vertical representative images.

Recommended image size:

- Portrait ratio, around `3:4`
- Suggested size: `900 x 1200px`
- File type: `.jpg` for photos, `.png` for screenshots or graphics
- Avoid very large files when possible; under `2 MB` is ideal

## Where Images Should Go

Publication cover images should be stored in:

```text
assets/publications/
```

Artwork cover images should be stored in:

```text
assets/artworks/
```

## File Naming

Use lowercase words separated by hyphens.

Good examples:

```text
generative-multi-sensory-meditation-cover.jpg
digital-mustard-garden-cover.jpg
see-my-sea-cover.jpg
common-pusher-cover.jpg
```

Avoid spaces, Chinese punctuation, parentheses, and special symbols in file names.

## How the Website Uses the Cover

Each item has an image line in `index.html`.

Publication example:

```html
<img class="publication-image" src="assets/publications/example-cover.jpg" alt="Representative image for Paper Title" width="180" height="240" loading="lazy">
```

Artwork example:

```html
<img class="artwork-image" src="assets/artworks/example-cover.jpg" alt="Representative image for Artwork Title" width="180" height="240" loading="lazy">
```

To replace a cover, only the `src` value needs to change.

## Replacement Checklist

After replacing a cover image:

1. Confirm the image file is in the correct folder.
2. Confirm the `src` path in `index.html` matches the file name exactly.
3. Open the local website preview.
4. Check that the cover loads in the correct item.
5. Check the mobile layout.
6. Commit and push the update to GitHub.

## Current Cover Folders

Publication covers:

```text
assets/publications/
```

Artwork covers:

```text
assets/artworks/
```

If a cover was generated from a PDF, it usually ends with:

```text
-cover.png
```

If a cover is manually uploaded, either `.jpg` or `.png` is fine.
