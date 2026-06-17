# Project Context

This project is the landing page for Shiran's advanced woven wrap workshop (`סדנת ארוג ארוך למתקדמות`).

Current status:
- The active branch remains `main`; no new branch was opened in this session.
- The site is still a single-page landing page implemented in `index.html`, with `header.jpeg` as the main image asset.
- The page remains Hebrew and RTL via `lang="he" dir="rtl"`.
- The visual system remains the warm golden / yellow / olive palette introduced in the previous updates.
- The documentation folder used to be `codex` and was renamed in this session to `docs`.

Current landing page structure:
- sticky topbar with hamburger button and drawer menu
- hero
- next workshop
- about
- learn
- register form
- success overlay
- videos
- cancellation policy
- social links
- footer

Cancellation policy change:
- A new cancellation policy section was added in `index.html` at lines `443-465`.
- The section was inserted between `#videos` and `#social`.
- The current page does not contain a visible FAQ section, so the new policy was placed in the intended near-end FAQ area before the social/footer ending flow.

Styling approach:
- Reused the existing `.card` section container so the new block keeps the same spacing, radius, and shadow language as the rest of the page.
- Added `.policy-intro`, `.policy-list`, and `.policy-item` in `index.html` lines `166-178`.
- The policy rows use the existing palette tokens (`--tz-200`, `--tz-300`, `--tz-800`, `--ink`) and a light bordered card treatment so the section feels official but still warm.

Behavior intentionally left unchanged:
- drawer open/close behavior and smooth-scroll handling
- PayBox redirect flow
- Formspree form action and silent submit iframe
- Google Apps Script API URL and request logic
- registration limit logic, past-date handling, and `FORCE_CLOSE` behavior
- edit mode (`?edit=1`) and `window.saveToGitHub` logic

Content/layout intentionally left unchanged outside the new section:
- workshop date
- workshop price
- form fields
- WhatsApp links
- PayBox URL
- Formspree URL
- Apps Script API URL
- existing section order aside from inserting the new cancellation policy block near the end
