# Gumlet (gumlet)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
