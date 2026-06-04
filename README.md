# King Saud University (king-saud-university)

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
