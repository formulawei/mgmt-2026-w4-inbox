# MGMT 2026 W4 interactive website — test report

status: static-verification-passed
updated: 2026-09-30

## Passed

- Inline JavaScript compiles in Node's JavaScript parser.
- HTML contains eight sequential activity stages.
- All HTML IDs are unique.
- Required prompt, progress, import, and export controls are present.
- Version 2 contains 119 bilingual content nodes and 35 response-field declarations; graph interactions and two reasoning rounds require live browser verification.
- The restricted article URL and source identifier are absent.
- No bilingual element contains child markup that would be destroyed by language switching.
- `index.html` and the standalone HTML copy are byte-identical.
- The GitHub Pages ZIP passes integrity testing.

## Browser automation limitation

The Playwright test script was prepared, but the execution environment has no installed Chromium binary and network installation is unavailable. Therefore the following require final verification in Chrome or Edge:

- Complete click-through of all unlock conditions.
- Actual download events for HTML, Markdown, and JSON.
- JSON re-import.
- Persistence after browser reload.
- Projection and mobile-device appearance.

The browser test can be rerun with `node test_w4_e2e.js` in an environment with Playwright Chromium installed.
