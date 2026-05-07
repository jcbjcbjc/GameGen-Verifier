# Example Task Descriptions

This directory holds **10 example** game-design Markdown files that the
pipeline can ingest. They are intended to demonstrate the input format and to
let reviewers reproduce a small slice of the pipeline end-to-end; they are
**not** the full benchmark.

Each file is named `<game_name>.md` and is consumed by:

- `scripts/prepare/generate_games.py`     — produce a runnable game project
- `scripts/prepare/distill_keypoints.py`  — extract verifiable keypoints
- `scripts/prepare/export_clean_games.py` — produce hook-stripped copies under `games_clean/`

Drop in your own `<game_name>.md` and the pipeline will pick it up — no other
registration is required.
