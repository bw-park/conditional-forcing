# Conditional Forcing

Project website for **Conditional Forcing: Long-Horizon Autoregressive Video Generation**.

Published with GitHub Pages at https://bw-park.github.io/conditional-forcing/.

## Local preview

```sh
python -m http.server 8000
```

Open http://localhost:8000/. No build step is needed.

## Publishing

GitHub Pages serves the root of the `main` branch. Changes pushed to `main` publish automatically. `.nojekyll` preserves the static assets as supplied.

All application and media paths are relative so the site works under a project subdirectory. Video uses HLS with local fMP4 segments, native browser playback when available, and the bundled hls.js fallback. Muted videos autoplay while visible; the gallery loads 12 cards at a time. Each video offers 1×, 2×, and 5× playback. Selections persist while navigating the page. Comparison videos synchronize when all rates match; different rates advance and loop independently while the shared seek and play/pause controls remain available.

The gallery contains 36 examples each for 30-second and 60-second rollouts. Matched comparisons include eight methods for six prompts. The training source code and manuscript are coming soon.

## Assets

`asset-sources.json` records the university logo sources. University marks identify author affiliations and belong to their respective institutions. The hls.js license is in `assets/vendor/`. Evaluation and qualitative examples originate from the project’s [Hugging Face gallery](https://huggingface.co/spaces/bw-park/cf-gallery-hq).
