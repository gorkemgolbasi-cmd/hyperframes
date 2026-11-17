---
description: Instagram Reels / TikTok vertical video from idea to a scheduled draft for review
argument-hint: <topic or idea>
---

Make a vertical (1080x1920) short video about: $ARGUMENTS

1. Use the `instagram-icerik` skill for hook, script and caption (Turkish unless told otherwise). Show it and wait for approval.
2. `/compact`, keeping only the approved script, caption and hashtags.
3. Build it with the `/yeni-video` flow at 1080x1920, 15–45 s, captions as an overlay (`captions-overlay`).
4. When `render-qa` passes, do NOT publish. Create a draft for review in the scheduling tool the user uses, at the best posting time if that tool can suggest one, and give the user the draft link.
