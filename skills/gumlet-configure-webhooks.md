---
name: gumlet-configure-webhooks
description: Register and verify Gumlet webhooks so an agent reacts to asset and live-stream events instead of polling.
api: gumlet:gumlet-webhooks-api
operations:
  - create-webhook
  - list-webhooks
  - update-webhook
  - delete-webhook
  - webhook-history
---

# Configure Gumlet webhooks

Subscribe to asynchronous events for video and live assets.

## Steps
1. Register an endpoint with `create-webhook` (`POST /org/webhooks`): supply `url`, a `secret_token`, the `triggers` (event types) and the `sources` to watch.
2. Confirm registration with `list-webhooks` (`GET /org/webhooks`).
3. On each delivery, verify authenticity: Gumlet echoes your secret token in the `x-gumlet-token` request header.
4. Return any `2xx` promptly. If you do not, Gumlet retries for 24 hours with ~30 minutes between attempts.
5. Inspect deliveries with `webhook-history` (`GET /org/webhook/{webhook_id}/history`); change or remove with `update-webhook` / `delete-webhook`.

## Event types
- Video: `video.status.created|stream_ready|downloaded|processed|ready|errored|deleted|repackaged`, `event.video.uploaded|updated`, `event.embed.viewed|cta_clicked|form_submitted`, `event.playlist.*`, `event.comment.all`, `event.channel.member_joined`.
- Live: `live.video.status.created|preparing|ready|connected|active|complete|disconnected`.
