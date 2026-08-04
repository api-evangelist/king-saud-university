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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

King Saud University (KSU) is a public research university in Riyadh, Saudi Arabia, founded in 1957 and ranked **#200 in the QS World University Rankings 2025**. This repository catalogs KSU's public developer/API footprint as an [APIs.json](http://apisjson.org) provider profile for the API Evangelist network. As of this review, KSU publishes no public, documented developer API — its digital services are end-user web applications gated behind institutional authentication.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=king-saud-university-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Saudi Arabia, Middle East, Research

## APIs

- **No Public Documented API** — KSU exposes no public, documented developer API. University services (Edugate SIS, LMS, library catalog, Saudi Digital Library access, manuscripts portal, e-services) require institutional SSO/login. Docs entry point: https://ksu.edu.sa/en

## Plans

- [plans/king-saud-university-plans-pricing.yml](plans/king-saud-university-plans-pricing.yml)

## Rate Limits

- [rate-limits/king-saud-university-rate-limits.yml](rate-limits/king-saud-university-rate-limits.yml)

## FinOps

- [finops/king-saud-university-finops.yml](finops/king-saud-university-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://ksu.edu.sa/en
- LinkedIn: https://www.linkedin.com/school/king-saud-university/
- Twitter/X: https://x.com/_KSU
- Authentication (Edugate SSO): https://edugate.ksu.edu.sa/ksu/init
- Review: [review.yml](review.yml)

## Notes

This profile reflects a strict no-fabrication review. All listed institutional endpoints (website, library affairs, Edugate, portal, faculty, Saudi Digital Library, manuscripts) were probed and resolve live, but none expose a documented public API, OpenAPI definition, or open-data API endpoint. A DSpace institutional repository is referenced in third-party registries (ROAR), but its repository subdomain and OAI-PMH endpoint did not resolve at review time. No endpoints were invented. See [review.yml](review.yml) for per-URL HTTP status details.

## Maintainers

- Kin Lane — kin@apievangelist.com
