---
name: gumlet-set-up-live-stream
description: Create a live-streaming workspace and asset on Gumlet, start the stream, and complete it.
api: gumlet:gumlet-live-stream-assets-api
operations:
  - live-workspace-create
  - create-live-asset
  - start-live
  - get-live-asset-status
  - complete-live-stream
---

# Set up a live stream on Gumlet

Provision and run a live-streaming session.

## Steps
1. Create a live workspace with `live-workspace-create` (`POST /video/sources/live`) to get a `live_source_id`.
2. Create the live asset with `create-live-asset` (`POST /video/live/assets`), passing `live_source_id`, `resolution`, and `title`. The response includes the ingest/playback details.
3. Start it with `start-live` (`POST /video/live/assets/{live_asset_id}/start`).
4. Monitor with `get-live-asset-status` (`GET /video/live/assets/{live_asset_id}`) or the `live.video.status.*` webhooks.
5. End the session with `complete-live-stream` (`POST /video/live/assets/{live_asset_id}/complete`).

## Conventions
- Auth: `Authorization: Bearer <API_KEY>`. Base URL `https://api.gumlet.com/v1`.
- Live events are delivered via webhooks: `live.video.status.created|preparing|ready|connected|active|complete|disconnected`.
