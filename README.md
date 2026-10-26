# King Saud University (king-saud-university)

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

King Saud University (جامعة الملك سعود, KSU) is Saudi Arabia's oldest public research university, founded in Riyadh in 1957. This repository catalogs KSU's public programmable footprint as an [APIs.json](http://apisjson.org) provider profile for the API Evangelist network.

**This profile was re-run on 2026-09-01 under the university pipeline and the previous finding was reversed.** The 2026-06-03 review concluded KSU published no public API. That was wrong. KSU operates two public, machine-readable, institution-owned surfaces — an open-data distribution programme and its own OAuth 2.0 / OpenID Connect / SAML identity plane. Both were missed because all of their documentation is Arabic-only: `data.ksu.edu.sa/en/api/guide` returns 404 while `data.ksu.edu.sa/ar/api/guide` returns 200.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=king-saud-university-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Class:** `university` — Public Research University
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Public Research University, Saudi Arabia, Middle East, Riyadh, Open Data, Research Data, Identity Federation, Single Sign-On, Research, Linked Data

## Surfaces, and who operates each one

A university is a federation of buyers, so every surface here carries an `x-operator` saying who runs the thing the entry describes — not who we fetched it from.

| Surface | Operator | What it is |
|---|---|---|
| [KSU Open Data Distribution API](openapi/king-saud-university-open-data-openapi.yml) | `institution` | 852 dataset files, seven families, five formats, unauthenticated, on the university's own domain |
| [KSU Identity and Access Management](openapi/king-saud-university-identity-openapi.yml) | `institution` | The university's own OAuth 2.0 / OIDC / SAML plane at `iam.ksu.edu.sa`, with public discovery documents |
| KSU identity provider in eduGAIN | `federation` | `http://SSO.ksu.edu.sa/adfs/services/trust`, registered by the Saudi Maeen federation (SA-MIF) |
| Crossref membership | `registry` | Member 19827, DOI prefix `10.33948`, 1,521 DOIs |
| ROR identifier | `registry` | [`https://ror.org/02f81g417`](https://ror.org/02f81g417) |
| Blackboard LMS | `tenant` | `lms.ksu.edu.sa` CNAMEs to `ksu.blackboard.com` — Anthology's contract, KSU's hostname and identity |

No vendor contract is stored in this repository. The tenancy above is recorded as a relationship; the platform's specification belongs to the vendor's own profile.

### KSU Open Data

The Data Management Office (مكتب إدارة البيانات) publishes institutional open data on the university's own domain, in JSON, XML, RDF/XML, CSV and XLSX, with no authentication of any kind and a KSU-authored open-data licence. Seven dataset families cover enrolled students and graduates, faculty, administrative and technical staff, outbound scholarships, scientific research, student services and activities, and community service including the University Medical City. Coverage runs from Hijri year 1430/1431 AH through 1444 AH and on into Gregorian 2023-2025, on a declared annual cadence.

Verified live on 2026-09-01: 20 of 20 sampled files returned HTTP 200 with the correct content type; the 1444 AH employee dataset returned 11,709 records.

The university additionally documents a *filtered query* endpoint at `GET /api/views/data_api`. That route is dead — Drupal answers `{"message":"No route found for \"GET /api/views/data_api\""}` — so it is deliberately **not** described in the OpenAPI. See [lifecycle/](lifecycle/king-saud-university-lifecycle.yml).

- Portal: https://data.ksu.edu.sa/ar
- API guide (Arabic): https://data.ksu.edu.sa/ar/api/guide
- Reference PDF (KSU-DMO-OD-API v.1.2, 13 pages): https://data.ksu.edu.sa/sites/data.ksu.edu.sa/files/2024-04/KSU-DMO-OD-API%20v.1.2.pdf
- Open Data Licence: https://data.ksu.edu.sa/ar/node/1178

### KSU identity plane

`iam.ksu.edu.sa` is a PingFederate deployment that serves a complete OpenID Connect discovery document and RFC 8414 authorization-server metadata anonymously, alongside a live JWKS. It advertises PKCE (S256), pushed authorization requests, CIBA, the device grant, token exchange, introspection, revocation, and front- and back-channel logout. The same deployment is the SAML identity provider registered in eduGAIN.

**Discoverable is not open.** The registration endpoint the discovery document advertises returns 404 to an anonymous request, and the university publishes no documentation for this surface. It is described here because it is real and institution-operated, not because a third party can integrate with it.

- OIDC discovery: https://iam.ksu.edu.sa/.well-known/openid-configuration
- Authorization server metadata: https://iam.ksu.edu.sa/.well-known/oauth-authorization-server
- JWKS: https://iam.ksu.edu.sa/pf/JWKS

## What King Saud University does not publish

No developer portal. No English API reference. No OpenAPI, AsyncAPI or `apis.json` of its own. No `llms.txt`, no agent card, no `security.txt`, no status page, no changelog. No self-service client registration. The OpenAPI documents in [openapi/](openapi/) are API Evangelist's, derived from the university's own documentation and live probes — each one says so in its `x-provenance`.

Three previously-claimed surfaces are dead and are not carried as pointers: the DSpace repository and OAI-PMH endpoint at `repository.ksu.edu.sa` (NXDOMAIN, though ROAR record 3330 still lists it), the library catalogue at `catalog.library.ksu.edu.sa` (resolves, TCP connection fails), and `edugate.ksu.edu.sa` (timed out on three consecutive attempts, having returned 200 in June).

A Figshare tenancy was tested and **rejected**: `ksu.figshare.com` answers HTTP 202 with an AWS WAF challenge, but a control request to a deliberately nonexistent `*.figshare.com` subdomain returns the identical challenge. It is not evidence of a KSU tenancy, and none is recorded.

## Artifacts

- OpenAPI: [openapi/](openapi/) — open data and identity, with pristine pre-refine copies in [openapi/_original/](openapi/_original/)
- JSON Schema: [json-schema/king-saud-university-open-data-datasets-schema.json](json-schema/king-saud-university-open-data-datasets-schema.json) — eight record shapes derived from live 1444 AH data
- Examples: [examples/king-saud-university-open-data-examples.yml](examples/king-saud-university-open-data-examples.yml) — verbatim responses
- Authentication: [authentication/](authentication/) — including the verbatim OIDC and RFC 8414 discovery documents
- Scopes: [scopes/king-saud-university-scopes.yml](scopes/king-saud-university-scopes.yml)
- Conformance: [conformance/king-saud-university-conformance.yml](conformance/king-saud-university-conformance.yml) — education-regime standards, reward-only
- Lifecycle: [lifecycle/king-saud-university-lifecycle.yml](lifecycle/king-saud-university-lifecycle.yml)
- Plans: [plans/king-saud-university-plans-pricing.yml](plans/king-saud-university-plans-pricing.yml)
- Rate limits: [rate-limits/king-saud-university-rate-limits.yml](rate-limits/king-saud-university-rate-limits.yml)
- FinOps: [finops/king-saud-university-finops.yml](finops/king-saud-university-finops.yml)
- Review: [review.yml](review.yml) — per-URL HTTP status detail for both reviews

## Domain standards (Kin Score `education` regime)

Conformance is reward-only and evidenced, never asserted from prose. Confirmed: **SAML** (IdP entity in eduGAIN via Maeen) and **Crossref** (member 19827, prefix 10.33948). Not conformant, with reasons recorded: OAI-PMH (endpoint gone), DataCite (no membership — the university registers through Crossref), Shibboleth (the deployment is PingFederate, not Shibboleth), ORCID, SCIM, LTI, OneRoster, Ed-Fi, Caliper, QTI.

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-09-01

## Common Properties

- Website: https://ksu.edu.sa/en
- Open Data: https://data.ksu.edu.sa/ar
- API Reference (Arabic): https://data.ksu.edu.sa/ar/api/guide
- Identity Federation: https://technical.edugain.org/entities?id=671188
- Authentication: https://iam.ksu.edu.sa/.well-known/openid-configuration
- AI Policy: https://aio.ksu.edu.sa/ar/node/2976
- AI Tooling: https://thakaa.ksu.edu.sa/en
- Library: https://library.ksu.edu.sa/en
- News: https://news.ksu.edu.sa/ar
- LinkedIn: https://www.linkedin.com/school/king-saud-university/
- Twitter/X: https://x.com/_KSU

## Maintainers

- Kin Lane — kin@apievangelist.com
