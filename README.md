# Plain-loop experiments: interactive dashboard

A read-only view of preliminary experiments in which language models (Qwen3.8-Flash-Next, gpt-oss-20b) repeatedly edit a
Bayesian-optimization program for constrained discrete sequence design (Ehrlich functions). Each model-written program is scored on
practice problems and kept only if it improves; finished programs are scored on problems the search never saw (held-out).

**Preliminary results.** Most differences between models are within run-to-run noise (about 0.01 to 0.02 in gain over random search).

- Open `index.html` (or the published page). The tree shows every program a search tried; click one to see the model's explanation,
  the edits it proposed and its scores.
- Page code adapted from [zhouk2-blip/Spiral-site](https://github.com/zhouk2-blip/Spiral-site); see `CREDITS.txt`.
- `site-data.js` and `site-config.js` are generated from the experiment runs.
