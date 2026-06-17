# Change Log

## 2026-06-17 13:45 IDT

Files changed:
- `index.html`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Refined the cancellation policy text styling to match the basic workshop landing page more closely.
- Removed bold emphasis from the policy rule text so each rule now renders in plain weight.
- Replaced the intro em dash with a comma.
- Slightly increased the spacing between the intro paragraph and the policy list.

Notes:
- The cancellation policy remains after the restored FAQ and before social.
- No JavaScript logic was changed.
- Workshop date, price, form fields, WhatsApp links, PayBox URL, Formspree URL, Apps Script API URL, registration limit logic, drawer behavior, and edit-mode GitHub save logic were not modified.

## 2026-06-17 FAQ repair

Files changed:
- `index.html`
- `docs/context.md`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Investigated the missing FAQ section in Git history before editing the page.
- Identified commit `08521338ecb6bcec77aed652cfa83a6446eb332f` as the last commit containing the historical FAQ block.
- Identified commit `980685ad632096b506594ee14688ddadadc178e7` as the first commit where that FAQ block disappears from `index.html`.
- Restored the FAQ content exactly from the historical block in `08521338ecb6bcec77aed652cfa83a6446eb332f`, preserving the original Hebrew wording, item order, and HTML structure as closely as possible.
- Applied the minimal compatibility adjustment required to make the section live again:
  - removed the surrounding HTML comment wrapper from the historical block
  - inserted the restored section before the existing cancellation policy
- Final near-end page order is now:
  - `#videos`
  - `#faq`
  - `#cancellation-policy`
  - `#social`
  - footer

Notes:
- No commit on `main` contained a visible uncommented FAQ section; the exact FAQ content existed only as a commented block in history.
- The removal in `980685ad632096b506594ee14688ddadadc178e7` appears accidental or incidental to unrelated work. The commit message and current documentation do not mention any intentional FAQ removal.
- No JavaScript logic was changed.
- Workshop date, price, form fields, WhatsApp links, PayBox URL, Formspree URL, Apps Script API URL, registration limit logic, drawer behavior, and edit-mode GitHub save logic were not modified.

## 2026-06-17 11:50 IDT

Files changed:
- `index.html`
- `docs/context.md`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Simplified the cancellation policy styling so the refund rules now render as a clean official list instead of separate bordered cards.
- Added a hamburger drawer link to `#cancellation-policy` with the label `מדיניות ביטולים`.
- Aligned the policy structure and visual treatment as closely as possible with the basic workshop landing page while preserving this page's existing golden palette.

Notes:
- This advanced landing page still had no visible FAQ section at that time, so the cancellation policy remained between `#videos` and `#social`.
- No JavaScript logic was changed.
- Workshop date, price, form fields, WhatsApp links, PayBox URL, Formspree URL, Apps Script API URL, registration limit logic, drawer behavior, and edit-mode GitHub save logic were not modified.

## 2026-06-17

Files changed:
- `index.html`
- `docs/context.md`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Renamed the documentation folder from `codex` to `docs`.
- Added a new cancellation policy section to `index.html` after the intended FAQ area, inserted between `#videos` and `#social`.
- Added small supporting CSS for the new policy section: `.policy-intro`, `.policy-list`, and `.policy-item`.
- Reused the existing `.card` container and warm golden/yellow palette tokens so the new section matches the current landing page design language.

Notes:
- The page currently had no visible FAQ section at that time, so the cancellation policy was placed in the intended near-end FAQ slot before the social/footer ending flow.
- No JavaScript logic was changed.
- Workshop date, price, form fields, WhatsApp links, PayBox URL, Formspree URL, Apps Script API URL, registration limit logic, drawer behavior, and edit-mode GitHub save logic were not modified.

## 2026-05-30

Files changed:
- `index.html`
- `docs/context.md`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Replaced the root `--tz-*` palette scale from purple/lilac tones to a warm cream, yellow, golden, mustard, and olive-brown scale.
- Updated related semantic colors including `--ink`, `--muted`, shadow rgba values, and focus ring color.
- Replaced remaining hardcoded old palette areas and cool-tinted UI states where relevant, including:
  - sticky topbar background
  - drawer link background and hover
  - hero gradient
  - outline button hover
  - hero image fallback background
  - form field background
  - FAQ open state background
  - footer text color
  - social link hover background
- Kept existing inline `var(--tz-*)` usage intact so the page continues to inherit from the centralized palette.
- Updated palette comments so they describe the warm yellow/golden direction instead of purple/lilac.

Notes:
- Old purple/lilac hardcoded values were scanned and replaced where relevant in the landing page source.
- No behavior, layout, spacing, copy, RTL structure, or intended content changes were introduced as part of this task.

## 2026-05-30 Follow-up

Files changed:
- `index.html`
- `docs/context.md`
- `docs/change-log.md`
- `docs/verification.md`

What was updated:
- Refined the warm palette transition between the sticky top area, hero, and page background by slightly softening the lightest palette stops and extending the hero gradient down into the shared page background value.
- Improved the hamburger button styling with a warm pale fill, clearer olive-brown icon lines, subtle border/shadow treatment, and a matching hover/active state.
- Kept the changes CSS-only in the landing page source.

Notes:
- This follow-up was intended only to fix the unsmooth hero-to-page visual cut and the weak hamburger presentation from the first yellow conversion.
- No behavior, layout, spacing, copy, RTL structure, or intended JavaScript changes were introduced.
