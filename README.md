# Sonnet Insurance (sonnet-insurance)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
