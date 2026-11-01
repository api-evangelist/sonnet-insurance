# Sonnet Insurance

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

Sonnet Insurance is a Canadian direct-to-consumer digital property and casualty insurer launched in 2016 and a member of the Definity family of companies, underwriting its own auto, home, condo, tenant, landlord and pet policies through Sonnet Insurance Company. It sells auto, home, condo, tenant and landlord coverage in Ontario, Quebec, New Brunswick, Nova Scotia and Prince Edward Island, and home-only coverage in British Columbia and Alberta, positioning itself as "Canada's original digital-first home and auto insurance company" with a fully online quote-and-buy flow and licensed agents for support. Sonnet is an explicit direct writer -- its own FAQ states that "a third party -- even a licensed broker -- cannot purchase a Sonnet policy on your behalf" -- so it operates no broker or agency distribution channel and therefore no ACORD/AL3 agency-download path. Its API posture is closed -- no developer, developers, docs or api subdomain resolves in DNS, every first-party developer path probed returns HTTP 404, and no OpenAPI, Swagger, GraphQL, Postman collection, webhook catalog or partner technical onboarding surface is published. The only third-party integrations Sonnet describes -- the Kanetix.ca (RATESDOTCA) quote-and-buy partnership and the Sonnet Connect brand referral program -- are privately negotiated commercial arrangements with no public technical documentation. Two machine-readable surfaces do exist and are captured here. Sonnet serves a real llms.txt at www.sonnet.ca/llms.txt that declares per-agent AI-Training, AI-Generation, AI-Summarization and AI-Crawling directives (Allow for OpenAI, Google-DeepMind and Anthropic) alongside a curated reference-content index -- an AI consent signal rather than an API contract. And the secure.sonnet.ca quote-and-buy application is driven by an undocumented first-party REST/JSON surface under /api/v1 covering quoting, binding, policy servicing, payments and identity; it is observable from Sonnet's own public JavaScript bundle but carries no documentation, no specification and no third-party terms of use, so it is recorded as observed evidence, not as an integratable API.

**Areas:** Insurance · Canada · Property and Casualty · Auto Insurance · Home Insurance · Insurtech · Direct to Consumer · Underwriting · Claims

## Sonnet Insurance on APIs.io

Everything profiled for Sonnet Insurance is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/sonnet-insurance/](https://apis.io/providers/sonnet-insurance/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Sonnet Insurance Domain Security](https://apis.io/security/sonnet-insurance/sonnet-insurance-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.sonnet.ca/)
- [Sign up](https://www.sonnet.ca/get-a-quote)
- [Support](https://www.sonnet.ca/contact-us)
- [Blog](https://www.sonnet.ca/blog)
- [Terms of service](https://www.sonnet.ca/terms-of-use)
- [Privacy policy](https://www.sonnet.ca/privacy)

## API Evangelist rating

**Kin Score 11.9** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 56.3 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 7.1 |
| Access clarity | 27.6 |

**Agent readiness 2.2** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | yes |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 12.3** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/sonnet-insurance/](https://apis.io/providers/sonnet-insurance/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Sonnet Insurance: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/sonnet-insurance/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
