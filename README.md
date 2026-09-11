# Chirag Goyal — editorial website

Responsive, frontend-only website inspired by the editorial hierarchy and immersive imagery of Gates Notes, adapted to the supplied Chirag Goyal content master. Warm cream, charcoal, restrained deep green, Montserrat headlines and Proxima Nova body typography.

## Preview

Open `index.html` directly, or run `python3 -m http.server 4173 --bind 127.0.0.1` in this folder and visit http://127.0.0.1:4173.

## Included

- Home, My Journey, My Work, Ekjut Nepal, Impact, Stories, story detail and Collaborate pages.
- Separate story archive with topic filters, search, URL state and empty results.
- Expandable journey entries with working deep links.
- Responsive navigation, keyboard focus states, Escape dismissal and reduced-motion support.
- Collaboration introduction download. Nothing is submitted, stored or sent.
- Informational People Registry. No registration or personal-data collection.

## Editing

Content is in `app.js`: `milestones` is the curated chronology and `stories` is the independent archive. Add stories there using a unique ID and existing category. `style.css` contains all styling. HTML entry points share the same script and stylesheet. No build tooling, packages, analytics, CMS or backend is required. JavaScript is currently required to render page content.

The two original prototype folders and the supplied DOCX remain untouched. The redesigned website starts at the root `index.html`.

## Typography and imagery

Montserrat is bundled in `assets/fonts`. Proxima Nova resolves from an installed local font; the local demo font was not redistributed. For consistent Proxima Nova on other devices, provide licensed webfont files or an authorised Adobe Fonts kit and update the `@font-face` declaration. Montserrat is the fallback.

The supplied magazine portrait is included in `assets/chirag-goyal.jpg`. It is low-resolution and contains publication text; replace it with an approved, clean, higher-resolution portrait when available.

Nepal landscape imagery is remotely loaded from Unsplash: https://images.unsplash.com/photo-1544735716-392fe2489ffa . It is illustrative context, not documentary evidence of any project. The article explicitly identifies this. The remote image requires internet access; the layout keeps a green background if it cannot load. Use approved project photographs for future documentary stories.

## Content and future integration

Copy is adapted from `Chirag_Goyal_Website_Content_Master.docx`. Earlier organisations remain attributed to Chirag’s personal journey, separate from Ekjut. Quantitative impact claims were deliberately omitted pending verification. The story texts are short editorial adaptations of the supplied summaries, not invented interviews or field reporting. Confirm chronology and final copy before publication.

Contact details were not supplied, so the collaboration page provides an honest local introduction download instead of a fake submission. Add confirmed contact details when available. CMS publishing and registry infrastructure are intentionally deferred per the frontend-only request.

## Verification

All eight page types checked at widths 1440, 768, 390 and 320 px: no horizontal overflow and no JavaScript page errors. Verified mobile menu open/Escape close, archive filtering/search/reset, timeline deep links and toggling, unknown-story state, introduction download, loaded imagery, and internal link responses. Desktop and mobile screenshots were visually reviewed.
