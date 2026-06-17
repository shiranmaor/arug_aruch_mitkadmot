# Change Log

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
- The page currently has no visible FAQ section, so the cancellation policy was placed in the intended near-end FAQ slot before the social/footer ending flow.
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
