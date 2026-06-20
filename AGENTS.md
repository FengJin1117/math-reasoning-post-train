# Interface Guidelines

## Visual style

- Use light page backgrounds for the public showcase. Do not use black or near-black full-page or full-section backgrounds.
- The GaoKao answer-sheet pages should follow the visual style of `/data2/fwh/post-train/exp/gaokao_2026/qwen2.5-3b/report.html`: light gray page, white cards, blue accents, and red error states.
- Keep the landing page concise. Full questions and answers belong on dedicated candidate subpages, reached through explicit links.

## Answer-sheet behavior

- Render the answer sheet directly like the canonical `report.html`.
- Do not add question folding, expand-all, or collapse-all controls.
- Treat the local `summary.json` and `report.html` as the source of truth for scores, extracted answers, and per-question results.
