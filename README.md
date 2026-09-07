# Northridge

The porch light is on.

A small static place to arrive. One continuous page, no dependencies, no build step.

## Open it

Open `index.html` in a browser. The site works directly from the folder, including the Archives and its inspection controls. Keep the HTML files, stylesheet, and assets together.

## Files

- `index.html` — the complete arrival, destination signposts, conditions, notice, and Municipal Archives with four objects to inspect.
- `archives.html` — a compatibility redirect to `index.html#municipal-archives`, with a fallback link.
- `styles.css` — the shared design, responsive layouts, keyboard focus, and reduced-motion support.
- `assets/northridge-arrival.webp` — the town entrance illustration.
- `assets/municipal-archives.webp` — the Archives interior illustration.
- `.nojekyll` — lets GitHub Pages serve the files as written.
- `ARTWORK.md` — the image prompts and illustration notes.

This repository keeps the public files at the root so GitHub Pages can publish directly from `main` without a build step.

## Design choices

The arrival pairs readable prose with a modest framed view down the road. Blue-gray dusk gives way to a lighter municipal paper surface. The Archives is warmer, with a small persistent way back to town. Location descriptions share a continuous surface instead of a card grid.

Objects use native HTML `details` and `summary`: choose a label to inspect it; choose it again to close it. The Lantern starts open. Multiple objects can remain open so there is no forced sequence. The controls work with keyboard, touch, and assistive technology without JavaScript. There is no plot state, audio, tracking, third-party request, backend, authentication, or external font.

The four undeveloped destinations retain the supplied prose and appear as road signs rather than inactive buttons or broken links. The deeper archive is an honest expandable placeholder; it does not point to a missing page or expose the private repository.

## Copy and canon

The supplied v0 copy is preserved. The only added visible sentence is functional placeholder text, shown only when the deeper archive is opened: “The deeper archive is not connected yet.” Skip links and accessible labels are navigation aids. Illustrations establish rooms and streets without adding named characters, events, or lore.

## GitHub Pages

In Settings → Pages, choose **Deploy from a branch**, then select **main** and **/(root)** and save. Once GitHub finishes publishing, the site will be available at:

https://7wygg6bk2n-cmyk.github.io/Northridge/

All links and assets use relative paths, so the site works under the repository subpath. The text is present directly in the HTML; no JavaScript or sign-in is needed to read it. Whether a particular AI can retrieve the published address must still be tested with its web reader.

To connect the deeper archive later, replace the `records-threshold` disclosure in `index.html` with a normal link to the intended archive.

## Validation

Static checks passed for the combined page: main landmarks and headings, labels, unique IDs, all relative file references and fragment links, image dimensions and alternative text, and native disclosure structure. All 60 supplied copy fragments are present. The 11 declared text/background combinations checked exceed 4.5:1 contrast (the lowest is 5.07:1). Responsive layout, visible keyboard focus, and reduced-motion rules are included.

The public HTML, CSS, and two WebP images total about 544 KiB. Live browser testing was not performed; keyboard behavior is provided by the native HTML controls rather than custom scripts.

## Continuous walk

The Archives is part of the homepage HTML. Enter the Archives jumps to `#municipal-archives`; Return to Northridge jumps to `#destinations`. The farewell follows the Archives. The Archives illustration loads lazily. Original prose and native object disclosures are preserved. Readers that retrieve the homepage can receive the Archives text in the same document, though tool extraction and access still vary. No new location lore has been added.
