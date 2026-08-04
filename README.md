# University of Liverpool (university-of-liverpool)

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
