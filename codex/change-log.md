# Change Log

## 2026-05-30

Files changed:
- `index.html`
- `codex/context.md`
- `codex/change-log.md`
- `codex/verification.md`

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
