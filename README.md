# Dog API (dog-api)

The internet's biggest collection of open-source dog pictures. The Dog API (dog.ceo) serves over 20,000 dog images accessible by more than 120 breeds via a free, no-auth REST API that returns JSON. Optional alt-text variants pair every image URL with descriptive text for accessibility. The canonical implementation is the open-source PHP Symfony project at [ElliottLandsborough/dog-ceo-api](https://github.com/ElliottLandsborough/dog-ceo-api), MIT licensed.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Tags

- Dogs
- Images
- Open Data
- Open Source

## Timestamps

- **Created:** 2024-11-14
- **Modified:** 2026-05-30

## APIs

### Dog API

The Dog API (dog.ceo) is the internet's largest collection of open-source dog pictures, exposing over 20,000 images across 120+ breeds. The API requires no authentication and returns JSON. The canonical implementation is the open-source PHP Symfony project at github.com/ElliottLandsborough/dog-ceo-api, MIT licensed.

**Human URL:** [https://dog.ceo/dog-api/](https://dog.ceo/dog-api/)

**Base URL:** `https://dog.ceo/api`

#### Tags

- Dogs, Images, Open Data

#### Properties

- [Documentation](https://dog.ceo/dog-api/documentation)
- [GitHub Source](https://github.com/ElliottLandsborough/dog-ceo-api)
- [Source Images Repo](https://github.com/jigsawpieces/dog-api-images)
- [OpenAPI](openapi/dog-api.yml)
- [Spectral Rules](rules/dog-api-rules.yml)
- [JSON Schema](json-schema/)
- [JSON Structure](json-structure/)
- [JSON-LD](json-ld/dog-api.jsonld)
- [JSON-LD Context](json-ld/dog-api-context.jsonld)
- [Vocabulary](vocabulary/dog-api.yml)
- [Capabilities](capabilities/)
- [Plans & Pricing](plans/dog-api-plans-pricing.yml)
- [Rate Limits](rate-limits/dog-api-rate-limits.yml)
- [FinOps](finops/dog-api-finops.yml)

## Common Properties

- [Website](https://dog.ceo)
- [Documentation](https://dog.ceo/dog-api/documentation)
- [GitHub](https://github.com/ElliottLandsborough/dog-ceo-api)
- [MIT License](https://opensource.org/licenses/MIT)
- [MCP Server (Community)](https://github.com/JithunMethusahan/dog-api-mcp-community)
- [p5.js Example](https://editor.p5js.org/codingtrain/sketches/lQxT7PTKC)
- [Vanilla JS Example](https://codepen.io/elliottlan/pen/MNEWNx)
- [jQuery Example](https://codepen.io/elliottlan/pen/KOXKLG)
- [Flutter Example](https://github.com/LIVELUCKY/dogs)
- [Node.js Example](https://github.com/mrbrunelli/dog-time-decorator)

## Features

| Name | Description |
|------|-------------|
| No Authentication | Fully open API; no key, token, or login required to consume any endpoint. |
| 120+ Breeds, 20,000+ Images | Broad coverage of master breeds and sub-breeds curated from the jigsawpieces/dog-api-images dataset. |
| Alt-Text Variant | Every image-returning endpoint has an `/alt` sibling that pairs the URL with descriptive alt text for accessibility. |
| Random Sampling | Random selection is available across breeds, sub-breeds, and images, with optional counts up to the upstream limit. |
| Open-Source Implementation | PHP Symfony source code is MIT-licensed and self-hostable; cache and image storage are pluggable. |
| Simple Envelope | Every response uses a uniform `{message, status}` JSON envelope, with `code` added on error responses. |

## Use Cases

| Name | Description |
|------|-------------|
| Pet UI Components | Drop random dog imagery into web or mobile components, demos, and onboarding flows. |
| Accessibility Demos | Showcase or test alt-text rendering and screen-reader behavior with the `/alt` endpoint family. |
| API Workshops & Tutorials | Use as a zero-friction, no-auth example API when teaching REST consumption, MCP, or API mocking. |
| ML Vision Datasets | Pull breed-tagged dog photography as a permissive public dataset for vision model training and evaluation. |
| Mock & Contract Testing | A stable, public envelope makes the Dog API a useful upstream for Spectral, Microcks, and contract-testing exercises. |

## Integrations

| Name | Description |
|------|-------------|
| Naftiko | REST + MCP capability adapters published for Breeds, Images, and Info surfaces. |
| Microcks | OpenAPI ships with `x-microcks-operation` extensions and named default examples for direct mock import. |
| Spectral | A repo-local Spectral ruleset enforces Dog API path, summary, parameter, and schema conventions. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Dog API OpenAPI 3.1](openapi/dog-api.yml) — 24 operations across 3 tags (Breeds, Images, Info), with Microcks default examples and 8 component schemas.

### JSON Schema

- [BreedListResponse](json-schema/dog-api-breed-list-response-schema.json)
- [ImageResponse](json-schema/dog-api-image-response-schema.json)
- [ImageListResponse](json-schema/dog-api-image-list-response-schema.json)
- [StringResponse](json-schema/dog-api-string-response-schema.json)
- [StringListResponse](json-schema/dog-api-string-list-response-schema.json)
- [AltImage](json-schema/dog-api-alt-image-schema.json)
- [AltImageListResponse](json-schema/dog-api-alt-image-list-response-schema.json)
- [ErrorResponse](json-schema/dog-api-error-response-schema.json)

### JSON Structure

- [BreedListResponse](json-structure/dog-api-breed-list-response-structure.json)
- [ImageResponse](json-structure/dog-api-image-response-structure.json)
- [ImageListResponse](json-structure/dog-api-image-list-response-structure.json)
- [StringResponse](json-structure/dog-api-string-response-structure.json)
- [StringListResponse](json-structure/dog-api-string-list-response-structure.json)
- [AltImage](json-structure/dog-api-alt-image-structure.json)
- [AltImageListResponse](json-structure/dog-api-alt-image-list-response-structure.json)
- [ErrorResponse](json-structure/dog-api-error-response-structure.json)

### JSON-LD

- [Dog API JSON-LD](json-ld/dog-api.jsonld) — schema.org WebAPI descriptor for the provider.
- [Dog API Context](json-ld/dog-api-context.jsonld) — Per-property term mappings derived from the JSON Schemas.

### Examples

- [breed-images.json](examples/breed-images.json) — Hand-curated breed-images sample.
- [list-all-breeds.json](examples/list-all-breeds.json) — Hand-curated master breed list sample.
- [random-image.json](examples/random-image.json) — Hand-curated random image sample.
- [Per-schema example files](examples/) — One generated example per JSON Schema.

## Capabilities

Naftiko capabilities — one self-contained file per OpenAPI tag, each exposing both a REST adapter and an MCP adapter inline.

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Dog API — Breeds](capabilities/dog-api-breeds.yaml) | Dog API | 9 | Pet Content Developer, Data Explorer |
| [Dog API — Images](capabilities/dog-api-images.yaml) | Dog API | 13 | Pet Content Developer, Accessibility Engineer, ML Data Collector |
| [Dog API — Info](capabilities/dog-api-info.yaml) | Dog API | 2 | Pet Content Developer |

## Vocabulary

- [Dog API Vocabulary](vocabulary/dog-api.yml) — Unified taxonomy mapping 3 resources, 3 actions, 3 workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Dog API Rules](rules/dog-api-rules.yml) — 32 Spectral rules across 10 categories enforcing Dog API conventions (read-only GET, kebab-case paths, "Dog API" title/summary prefix, camelCase parameters and properties, `{message, status}` envelope, open security posture, Microcks extensions).

## Plans, Rate Limits, FinOps

- [Plans & Pricing](plans/dog-api-plans-pricing.yml) — API Commons Plans 0.1 scaffold (the hosted dog.ceo service itself is free; this captures a hypothetical paid surface for self-hosted or commercial mirrors).
- [Rate Limits](rate-limits/dog-api-rate-limits.yml) — API Commons Rate Limits 0.1 scaffold; no rate limits are published by dog.ceo, so the document captures recommended client-side conventions.
- [FinOps](finops/dog-api-finops.yml) — FOCUS-aligned FinOps Framework definition for tracking usage of the API surface in commercial deployments.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
