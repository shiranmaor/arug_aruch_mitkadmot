# Project Context

This project is the landing page for Shiran's advanced woven wrap workshop (`סדנת ארוג ארוך למתקדמות`).

Current status:
- The active branch remains `main`; no new branch was opened in this session.
- The site remains a single-page landing page implemented in `index.html`, with `header.jpeg` as the main image asset.
- The page remains Hebrew and RTL via `lang="he" dir="rtl"`.
- The visual system remains the warm golden / yellow / olive palette introduced in the previous updates.
- The documentation folder was previously renamed from `codex` to `docs`.

Current landing page structure:
- sticky topbar with hamburger button and drawer menu
- hero
- next workshop
- about
- learn
- register form
- success overlay
- videos
- FAQ
- cancellation policy
- social links
- footer

FAQ repair summary:
- At the start of this repair, the current page still had FAQ traces:
  - a drawer link to `#faq`
  - existing FAQ CSS for `details`, `summary`, and `.faq-body`
  - but no live FAQ section in the page markup
- Git investigation found that the exact historical FAQ content exists in commit `08521338ecb6bcec77aed652cfa83a6446eb332f`, but only as a commented HTML block.
- Commit `980685ad632096b506594ee14688ddadadc178e7` is the first commit where that historical FAQ block disappears entirely from `index.html`.
- No commit on `main` contained an uncommented visible FAQ section; the restoration therefore reused the exact historical FAQ content and removed only the surrounding HTML comment markers so it could render again.
- The restored FAQ section now appears in [index.html](/home/matan/Documents/shiran/arug_aruch_mitkadmot/index.html:450) at lines `450-469`.
- The cancellation policy remains the same block and now follows the FAQ at [index.html](/home/matan/Documents/shiran/arug_aruch_mitkadmot/index.html:471), producing the intended ending flow:
  - videos
  - FAQ
  - cancellation policy
  - social
  - footer

Historical FAQ source restored:
- Source commit: `08521338ecb6bcec77aed652cfa83a6446eb332f`
- Restored heading: `שאלות נפוצות`
- Restored item order and wording:
  - `האם צריך להביא מנשא?`
  - `מאיזה גיל אפשר?`
  - `מה אם כואב לי הגב כשאני נושאת?`
  - `אפשר להגיע עם תינוק ישן/רעב?`

Styling approach:
- Reused the existing FAQ CSS already present in `index.html` lines `159-164`.
- No new FAQ styling was added.
- The restored section inherits the current golden/yellow/olive palette through existing variables and card styles.

Behavior intentionally left unchanged:
- drawer open/close behavior and smooth-scroll handling
- PayBox redirect flow
- Formspree form action and silent submit iframe
- Google Apps Script API URL and request logic
- registration limit logic, past-date handling, waiting-list logic, and `FORCE_CLOSE` behavior
- edit mode (`?edit=1`) and `window.saveToGitHub` logic

Content/layout intentionally left unchanged outside the FAQ repair:
- workshop date
- workshop price
- form fields
- WhatsApp links
- PayBox URL
- Formspree URL
- Apps Script API URL
- cancellation policy content
