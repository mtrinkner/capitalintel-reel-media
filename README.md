# capitalintel-reel-media

Durable media hosting for scheduled [@capitalintel.ai](https://instagram.com/capitalintel.ai) reels.

Buffer ingests video **by URL at publish time**, so a reel's MP4 must stay reachable from the
moment it is scheduled until the moment it publishes. Free ephemeral hosts (litterbox 72h,
uguu 3h) expire or go down, which caused a failed publish on 2026-07-22. Release assets in
this repo do not expire, so no watchdog process — and no machine left awake — is required.

Assets live under the `media` release tag and are uploaded by `src/publishing/videoHost.ts`.

## Footage rights

Clips are sourced from each featured company's own official channels and are used for
editorial commentary, with the source credited in every post caption. Rights status is
tracked per reel as `official-review-required`. If you are a rights holder and want a clip
removed, open an issue and it will be deleted.
