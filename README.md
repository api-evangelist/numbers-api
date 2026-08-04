# Numbers API

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

Free REST API providing interesting mathematical facts, trivia, dates, and year facts about numbers for educational and fun applications.

## Overview

The Numbers API returns short, readable facts about any number or date across four categories: trivia, mathematical properties, notable years, and day-of-year historical events. No authentication or API key is required.

**Base URL:** `http://numbersapi.com`

**Creator:** David Hu and Mack Duan

## Endpoints

| Endpoint | Description |
|----------|-------------|
| `/{number}` | Trivia fact about a number |
| `/{number}/trivia` | Trivia fact about a number (explicit) |
| `/{number}/math` | Mathematical property of a number |
| `/{number}/year` | Notable historical event for a year |
| `/{month}/{day}/date` | Historical fact for a calendar date |
| `/random` | Random fact (any type) |
| `/random/trivia` | Random trivia fact |
| `/random/math` | Random math fact |
| `/random/year` | Random year fact |
| `/random/date` | Random date fact |

## Response Formats

- **Plain text** (default): A single readable sentence
- **JSON** (append `?json`): Structured object with fields `text`, `number`, `type`, and `found`

## Authentication

None required. No API key, no signup, no token.

## Pricing and Rate Limits

The Numbers API is completely free with no published rate limits. It operates as a community resource on a best-effort basis. Caching is strongly recommended.

## Repository Contents

- `apis.yml` — APIs.json 0.19 profile
- `plans/numbers-api-plans-pricing.yml` — Pricing plan details
- `rate-limits/numbers-api-rate-limits.yml` — Rate limit policies
- `finops/numbers-api-finops.yml` — FinOps guidance for consumers

## Links

- Website: http://numbersapi.com
- Documentation: http://numbersapi.com/#42
