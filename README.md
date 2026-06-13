# Numbers API

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
