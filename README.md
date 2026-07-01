# Gumlet (gumlet)

Gumlet is a video hosting, streaming, and image optimization platform. Its video APIs cover on-demand and live streaming, per-title encoding, DRM, subtitles, and analytics, while its image APIs provide real-time resize, compression, and CDN delivery from cloud storage sources. All surfaces run under a single REST API at api.gumlet.com/v1 authenticated with a bearer API key.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/apis.yml)

## Tags

- Video
- Streaming
- Image Optimization
- CDN
- Encoding
- Analytics

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Gumlet Video Assets API

Ingest, encode, and manage video-on-demand assets with adaptive bitrate (HLS/DASH) or MP4 output, per-title encoding, DRM, overlays, trimming, subtitles, chapters, and thumbnails.

- **Human URL:** [https://docs.gumlet.com/reference/create-asset](https://docs.gumlet.com/reference/create-asset)
- **Base URL:** `https://api.gumlet.com/v1/video`

#### Tags

- Video
- Assets
- Encoding
- VOD

#### Properties

- [Documentation](https://docs.gumlet.com/docs/video-getting-started)
- [API Reference](https://docs.gumlet.com/reference/create-asset)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gumlet Video Collections API

Create and manage video collections (sources) that group assets under a workspace, along with playlists and folders for organizing library content.

- **Human URL:** [https://docs.gumlet.com/reference/list-collections](https://docs.gumlet.com/reference/list-collections)
- **Base URL:** `https://api.gumlet.com/v1/video`

#### Tags

- Video
- Collections
- Sources
- Workspaces

#### Properties

- [Documentation](https://docs.gumlet.com/docs/manage-sources)
- [API Reference](https://docs.gumlet.com/reference/list-collections)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gumlet Live Streaming API

Create and manage live streaming assets with RTMP ingest, live-to-VOD recording, status history, and thumbnails for real-time broadcast workflows.

- **Human URL:** [https://docs.gumlet.com/reference/create-live-asset](https://docs.gumlet.com/reference/create-live-asset)
- **Base URL:** `https://api.gumlet.com/v1/video`

#### Tags

- Live
- Streaming
- RTMP
- Low Latency

#### Properties

- [Documentation](https://docs.gumlet.com/docs/live-streaming)
- [API Reference](https://docs.gumlet.com/reference/create-live-asset)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gumlet Image Optimization API

Manage image sources that connect cloud storage (S3, GCS, Spaces, Wasabi) to Gumlet's real-time resize, compression, format conversion, and CDN delivery, including cache purging.

- **Human URL:** [https://docs.gumlet.com/docs/manage-sources](https://docs.gumlet.com/docs/manage-sources)
- **Base URL:** `https://api.gumlet.com/v1`

#### Tags

- Image
- Optimization
- Sources
- CDN

#### Properties

- [Documentation](https://docs.gumlet.com/docs/image-getting-started)
- [API Reference](https://docs.gumlet.com/docs/image-transform-apis)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gumlet Analytics API

Query video and image analytics with aggregated, breakdown, and chart data APIs covering views, unique viewers, watch time, and engagement/completion metrics.

- **Human URL:** [https://docs.gumlet.com/docs/advanced-video-analytics](https://docs.gumlet.com/docs/advanced-video-analytics)
- **Base URL:** `https://api.gumlet.com/v1`

#### Tags

- Analytics
- Insights
- Engagement
- Views

#### Properties

- [Documentation](https://docs.gumlet.com/docs/advanced-video-analytics)
- [API Reference](https://docs.gumlet.com/docs/insights-metrics-tracked)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gumlet Uploads API

Request signed direct-upload URLs and complete multipart uploads to ingest local video files into Gumlet for processing.

- **Human URL:** [https://docs.gumlet.com/reference/create-asset-direct-upload](https://docs.gumlet.com/reference/create-asset-direct-upload)
- **Base URL:** `https://api.gumlet.com/v1/video`

#### Tags

- Uploads
- Direct Upload
- Multipart

#### Properties

- [Documentation](https://docs.gumlet.com/docs/direct-upload)
- [API Reference](https://docs.gumlet.com/reference/create-asset-direct-upload)
- [OpenAPI](openapi/gumlet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gumlet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gumlet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/gumlet)
- [LinkedIn](https://www.linkedin.com/company/gumlet)
- [Website](https://www.gumlet.com/)
- [Documentation](https://docs.gumlet.com/)
- [Plans](plans/gumlet-plans-pricing.yml)
- [Rate Limits](rate-limits/gumlet-rate-limits.yml)
- [Fin Ops](finops/gumlet-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
