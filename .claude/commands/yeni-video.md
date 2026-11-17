---
description: New HyperFrames video end to end — brief, scaffold, compose, gates, render
argument-hint: <brief or path to a brief .md>
---

Make a new HyperFrames video from this brief: $ARGUMENTS

1. Load `/hyperframes`. Turn the brief into a short script + storyboard (format, duration, scenes, VO yes/no). Show it and wait for approval.
2. After approval, run `/compact` keeping only: approved storyboard, format, duration, output path.
3. Scaffold with `npx hyperframes init <dir> --skip-skills`. Use `/hyperframes-registry` before hand-building any named visual and `/media-use` for VO, music, images.
4. Hand scene motion to the `motion-director` agent.
5. Hand gates to the `render-qa` agent. Fix what it reports, repeat until PASS.
6. Run `/compact` again, then render: `npx hyperframes render --quality draft -o out/draft.mp4`; after approval `--quality delivery -o out/final.mp4`.
7. Send the final file through `render-qa` once more and give the path.
