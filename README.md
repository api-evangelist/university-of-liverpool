# University of Liverpool (university-of-liverpool)

The University of Liverpool is a public research university in Liverpool, United Kingdom, a founding member of the Russell Group, ranked #165 in the QS World University Rankings 2025. This repository catalogs the institution's public, machine-readable developer/API footprint as an [APIs.json](https://apisjson.org) profile. That footprint is centered on scholarly and research-data infrastructure: two live OAI-PMH metadata-harvesting interfaces. No unified public API developer portal was found at the time of review.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-liverpool/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-liverpool-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- OAI-PMH
- United Kingdom

## APIs

- **University of Liverpool Repository OAI-PMH** — OAI-PMH 2.0 interface for the EPrints-based open-access research repository. Base URL: `https://livrepository.liverpool.ac.uk/cgi/oai2`. Docs: https://livrepository.liverpool.ac.uk/information.html
- **DataCat Research Data Catalogue OAI-PMH** — OAI-PMH 2.0 interface for the EPrints-based research data catalogue. Base URL: `https://datacat.liverpool.ac.uk/cgi/oai2`. Docs: http://datacat.liverpool.ac.uk/information.html

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-liverpool-plans-pricing.yml](plans/university-of-liverpool-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-liverpool-rate-limits.yml](rate-limits/university-of-liverpool-rate-limits.yml)
- FinOps: [finops/university-of-liverpool-finops.yml](finops/university-of-liverpool-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.liverpool.ac.uk/
- GitHub: https://github.com/livuni
- LinkedIn: https://www.linkedin.com/school/university-of-liverpool/
- Review: [review.yml](review.yml)

## Notes

- All endpoints listed were probed live on 2026-06-03. Both OAI-PMH interfaces returned HTTP 200 and responded to the `Identify` verb; the Repository also returned its metadata formats via `ListMetadataFormats`.
- No public general-purpose API developer portal, course/timetable/SIS API, or self-service API key program was found to be publicly documented.
- The `livuni` GitHub org is a small academic/research org (mostly forks), not an official institutional API publisher.
- SSO/IdP and status hosts did not resolve publicly. No endpoints were fabricated — only verified URLs appear in this profile.

## Maintainers

- Kin Lane — kin@apievangelist.com
