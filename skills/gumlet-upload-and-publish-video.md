---
name: gumlet-upload-and-publish-video
description: Upload a video into a Gumlet workspace, track processing to ready, and publish it for embedding.
api: gumlet:gumlet-video-assets-api
operations:
  - create-asset
  - create-asset-direct-upload
  - get-asset-details
  - update-asset
  - upload-subtitles
---

# Upload and publish a video on Gumlet

Ingest a video-on-demand asset, wait for processing, and make it embeddable.

## Steps
1. Pick or create a workspace (see `list-workspaces` / `create-workspace`); you need a `collection_id`/`workspace_id`.
2. Ingest the source:
   - From a URL: `create-asset` (`POST /video/assets`) with the `input` URL and target `collection_id`/`profile_id`.
   - From a local file: `create-asset-direct-upload` (`POST /video/assets/upload`) to get a signed upload URL, then PUT the file to it.
3. Poll `get-asset-details` (`GET /video/assets/{asset_id}`) until status is `ready`. Or subscribe to the `video.status.ready` webhook (see the webhooks skill) instead of polling.
4. Enrich metadata with `update-asset` (`POST /video/assets/update`): title, description, tags, call_to_actions.
5. Optionally add captions with `upload-subtitles`, then confirm with `complete-subtitle-upload`.

## Conventions
- Auth: `Authorization: Bearer <API_KEY>`. Base URL `https://api.gumlet.com/v1`.
- No idempotency key is supported; do not blindly retry a create on timeout — reconcile with `get-asset-details` first.
- Deletes are recoverable: a deleted asset can be restored with `recover` from the recycle bin.
