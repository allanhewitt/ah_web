# B1700 presentation publication

Published portal: https://allanhewitt.github.io/ah_web/b1700-presentations/

Source copies of the 2026–27 presentations came from Dropbox /Teaching/2026-27/B1700/presentations/weekXX/; the Dropbox originals are unchanged.

The six Quarto source copies use the shared `../styles.css` stylesheet (all six Dropbox stylesheet files were verified identical) and add `embed-resources: true` to the RevealJS config. This produces a single-file HTML presentation with CSS, JavaScript and diagrams embedded.

Edit the source copies, SVGs or shared CSS in GitHub and the build workflow `.github/workflows/build-b1700-presentations.yml` will render the six decks and commit the `weekXX_slides.html` files. GitHub Pages serves the HTML files from `main`. The original B1700 task and hint pages are unchanged.

For enrolled students, add the individual presentation URLs or portal URL as URL resources in Myplace rather than uploading the HTML file.
