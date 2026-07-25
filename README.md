# Sonnet Insurance (sonnet-insurance)

Sonnet Insurance is a Canadian direct-to-consumer digital property and casualty insurer launched in 2016 and a member of the Definity family of companies, underwriting its own auto, home, condo, tenant, landlord and pet policies through Sonnet Insurance Company. It sells auto, home, condo, tenant and landlord coverage in Ontario, Quebec, New Brunswick, Nova Scotia and Prince Edward Island, and home-only coverage in British Columbia and Alberta.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sonnet-insurance/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sonnet-insurance/refs/heads/main/apis.yml)

## Tags

- Insurance
- Canada
- Property and Casualty
- Auto Insurance
- Home Insurance
- Insurtech
- Direct to Consumer
- Underwriting
- Claims

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

Sonnet Insurance publishes **no public API**. This entry is intentionally empty, and that absence is the finding.

Every candidate developer host — `developer.sonnet.ca`, `developers.sonnet.ca`, `docs.sonnet.ca`, `api.sonnet.ca` — fails to resolve in DNS. Every candidate first-party path — `/developers`, `/developer`, `/api`, `/partners`, `/integrations` — returns HTTP 404. `/openapi.json`, `/swagger.json`, `/api-docs`, `/graphql`, `/.well-known/openid-configuration` and `/.well-known/oauth-authorization-server` all return HTTP 404. The published sitemap contains no developer, docs or API path. No OpenAPI, Swagger, AsyncAPI, GraphQL SDL, Postman collection, webhook catalog, SDK or GitHub organization exists.

### ACORD posture

**No ACORD reference found.** Searches for ACORD, AL3, ACORD XML, NGDS, IVANS, Applied Epic, Vertafore and AMS360 return nothing across Sonnet's site. This is structural rather than accidental: Sonnet is an explicit direct writer with no broker or agency channel — its own FAQ states that "a third party – even a licensed broker – cannot purchase a Sonnet policy on your behalf" — so the ACORD agency-download rails that carry integration for broker-distributed Canadian carriers have nothing to attach to here.

### Quote / bind / issue / FNOL

Sonnet genuinely does all four online, and is notable in the Canadian market for allowing full purchase (not just quoting) through the Kanetix.ca comparison platform. But all four run exclusively inside Sonnet's own first-party web application at `www.sonnet.ca`. None is exposed as a documented API to consumers, agents or partners.

The only third-party integrations Sonnet describes are commercial, not technical: the Kanetix.ca (RATESDOTCA) quote-and-buy partnership and the Sonnet Connect brand referral program, neither of which publishes any integration detail.

### Two machine-readable surfaces that do exist

**An `llms.txt`, but no API.** `https://www.sonnet.ca/llms.txt` returns a real 5,836-byte document declaring per-agent AI directives — `AI-Training`, `AI-Generation`, `AI-Summarization` and `AI-Crawling` all set to `Allow`, with named entries for OpenAI, Google-DeepMind and Anthropic — plus a curated index of Sonnet's product, support, legal and social pages and a "Sitemap for AI Indexing (Not Training)" pointer. A carrier with no developer program has nonetheless published a deliberate agent-facing consent posture. The AI surface arrived before the API surface. Captured verbatim in `llms/`.

**An undocumented internal API.** DNS enumeration surfaced `secure.sonnet.ca` — the only resolving non-`www` subdomain and the host of Sonnet's AngularJS quote-and-buy application. Its public application bundle contains **117 distinct `/api/v1/*` endpoint paths** spanning quoting (30), identity and verification (21), payments and billing (14), underwriting data (11), policy servicing (10), binding and issuance (7), address and availability (7), customer profile (7), group discounts (4), content and support (4), claims (1) and telemetry (1). `/api/v1/digital_quotes/create_auto`, `/api/v1/bind_policy` and `/api/v1/generate_document/` mean quote, bind and issue are each backed by real JSON endpoints. No FNOL endpoint was observed.

This does not make Sonnet an API provider. There is no documentation, no specification, no developer terms and no credential a third party can obtain. Nothing was called and nothing was inferred: the inventory in `endpoints/` records observed paths only, `apis[]` stays empty, and no OpenAPI was fabricated.

### Market context

Canada has the most fragmented insurance supervision of the major markets — OSFI supervises federally-regulated insurers prudentially while the provinces regulate market conduct (FSRA in Ontario, AMF in Quebec). There is no open-insurance mandate, and Consumer-Driven Banking, Canada's open-banking framework, excludes insurance entirely. Nothing compels Sonnet to expose an API, and it does not.

## Links

- [Website](https://www.sonnet.ca/)
- [About](https://www.sonnet.ca/about-us)
- [Blog](https://www.sonnet.ca/blog)
- [Partnerships](https://www.sonnet.ca/partnerships)
- [Account Login](https://www.sonnet.ca/account-log-in)
- [LinkedIn](https://www.linkedin.com/company/sonnet-insurance)
- [X](https://x.com/sonnetinsurance)

## Maintainers

- Kin Lane — kin@apievangelist.com
