# Thai Recall

A static, no-account Thai vocabulary trainer. 210 records extracted from all 22 pages of the supplied Thai.pdf. All English meanings, romanizations and example sentences retain the source wording and tone marks. Thai text is internal only. Distinct examples are retained.

## Run locally

Run `python -m http.server 8000` in this folder, then open http://localhost:8000. Do not open index.html directly: browsers restrict JSON loading from file URLs.

## Publish free on GitHub Pages

1. Create a public GitHub repository named `thai-recall`.
2. Upload index.html, style.css, app.js, data.json, the audio folder, and .nojekyll to its root. Preserve the audio folder structure (GitHub Desktop is convenient for uploading the full folder).
3. In Settings → Pages, select Deploy from a branch, branch main, folder /(root), then Save.
4. Open the HTTPS address shown by GitHub Pages once deployment finishes: https://omriaviam.github.io/thai-recall/ if using that account and repository name.

No build, dependencies, API keys, paid service or registration is required at runtime. Google Fonts is optional; system fonts are the fallback.

## Practice and progress

Tap the English meaning to reveal the pronunciation and example. Listen plays a bundled MP3 generated from the PDF's Thai spelling. Again schedules 10 minutes; A little tricky schedules 1 day; Got it starts at 3 days and doubles successful intervals up to 180 days. Due for review includes unseen words. All words permits unrestricted browsing. Saved words is independent of scheduling. Browsing alone never marks a word learned. Space reveals; arrow keys navigate.

Progress is local to each browser and origin. Export/import transfers it to another device or hosting address. Clearing browser data removes local progress.

## Audio and source fidelity

Audio uses Microsoft Thai neural TTS: Premwadee, with Niwat for w073. MP3 files are bundled so visitors need no installed Thai voice. PDF extraction artifacts involving Thai sara am and line breaks were normalized for synthesis; the original extracted spelling remains in data.json. English and romanized content was not translated or rewritten. The source itself may contain linguistic inconsistencies; fidelity to the supplied document does not constitute a native-speaker accuracy review. The synthesized audio has not been independently certified by a native Thai speaker.

Source PDF is not redistributed. Keep only the application files above in the Pages deployment; preview PNGs and this README are optional.
