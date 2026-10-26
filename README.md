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

The University of Liverpool is a public research university in Liverpool, United Kingdom, a founding member of the Russell Group. This repository catalogs the institution's public, machine-readable footprint as an [APIs.json](https://apisjson.org) profile, under the API Evangelist **university pipeline** — which settles *who operates* each surface before recording it, because most of what appears under a university's name is a vendor's contract running on the institution's behalf.

The institution runs no public developer portal, publishes no OpenAPI and issues no API keys. What it does operate, on its own hosts, are five machine surfaces: two EPrints OAI-PMH 2.0 providers, a keyless EPrints REST read interface, an AD FS OAuth 2.0 / OpenID Connect authorization server with public discovery and JWKS, and a Shibboleth SAML 2.0 identity provider published in the UK Access Management Federation. Four registry memberships and four vendor tenancies are recorded separately, as relationships rather than as Liverpool's engineering.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-liverpool/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-liverpool-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party — `x-type: university`, `x-category: Public Research University`

## Tags

- Education
- Higher Education
- University
- Russell Group
- United Kingdom
- Research
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- EPrints
- Identity Federation
- Library
- Metadata

## Surfaces, by operator

Every entry in `apis.yml` carries an `x-operator`. `institution` means the university runs the thing; `federation` means a shared identity federation carrying the university's own IdP; `registry` means an identifier registry the university is registered in; `tenant` means the data is the university's and the contract is a vendor's.

### institution

- **University of Liverpool Repository OAI-PMH** — EPrints 3.4.5, eight metadata formats including RIOXX and uketd_dc. `https://livrepository.liverpool.ac.uk/cgi/oai2`
- **University of Liverpool Repository EPrints REST** — keyless read; `GET /rest/eprint/` returns 7.4MB of eprint ids with no credentials. `https://livrepository.liverpool.ac.uk/rest/`
- **DataCat Research Data Catalogue OAI-PMH** — EPrints 3.4.4 research data catalogue. `https://datacat.liverpool.ac.uk/cgi/oai2`
- **AD FS OAuth 2.0 / OpenID Connect** — public discovery and JWKS on the university's own host. `https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration`

### federation

- **Shibboleth IdP (UK Access Management Federation)** — entityID `urn:mace:eduserv.org.uk:athens:provider:liv.ac.uk`, served live by the federation MDQ and self-published at `https://shibboleth3.liv.ac.uk/idp/shibboleth`
- **Microsoft Entra ID tenant** — `53255131-b129-4010-86e1-474bfd7e8076`, discoverable by domain

### registry

- **DataCite** — repository member BL.LPOOL since 2015; prefix 10.17638; 16,405 DOIs resolving into livrepository
- **ORCID** — affiliation programme via the Jisc UK ORCID consortium; 13,225 records name the institution
- **ROR** — `04xs57h96`; Crossref Funder Registry 501100000836, GRID grid.10025.36, ISNI 0000 0004 1936 8470
- **Crossref** — member 2165, Liverpool University Press, prefix 10.3828, 114,739 DOIs

### tenant

- **Ex Libris Alma / Primo VE** — library discovery, `vid=44LIV_INST:LIV`
- **Talis Aspire** — reading lists; `https://liverpool.rl.talis.com/index.json` serves RDF/JSON
- **Instructure Canvas** — VLE on `canvas.liverpool.ac.uk`, live LTI 1.3 JWKS, data API closed (401)
- **Symplectic Elements** — Liverpool Elements CRIS, auth-gated (401)

## Artifacts

- Conformance (education regime): [conformance/university-of-liverpool-conformance.yml](conformance/university-of-liverpool-conformance.yml)
- Authentication: [authentication/university-of-liverpool-authentication.yml](authentication/university-of-liverpool-authentication.yml)
- Scopes: [scopes/university-of-liverpool-scopes.yml](scopes/university-of-liverpool-scopes.yml)
- Errors: [errors/university-of-liverpool-oai-error-codes.yml](errors/university-of-liverpool-oai-error-codes.yml)
- Plans & Pricing: [plans/university-of-liverpool-plans-pricing.yml](plans/university-of-liverpool-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-liverpool-rate-limits.yml](rate-limits/university-of-liverpool-rate-limits.yml)
- FinOps: [finops/university-of-liverpool-finops.yml](finops/university-of-liverpool-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.liverpool.ac.uk/
- Open Research: https://www.liverpool.ac.uk/open-research/
- AI policy: https://www.liverpool.ac.uk/about/the-university/reports-policies-and-governance/ai-at-liverpool/policies-and-guidance/
- GitHub: https://github.com/livuni
- LinkedIn: https://www.linkedin.com/school/university-of-liverpool/
- Review: [review.yml](review.yml)

## Notes

- All endpoints were probed live on 2026-09-01. **No OpenAPI has been generated for any of these surfaces**: the EPrints, Canvas, Alma, Talis and Elements contracts are product contracts shared by every deployment of that software, and belong in the vendor's own repo — not credited to Liverpool.
- Seven of the twelve Kin Score `education` regime domain standards are evidenced from live endpoints: `oai-pmh`, `shibboleth`, `saml`, `orcid`, `datacite`, `crossref`, and `lti` (the last on the Canvas tenant, not Liverpool's own engineering).
- **User-Agent trap:** `livrepository.liverpool.ac.uk` returns 403 to a desktop-browser User-Agent on every path and 200 to curl's default or an OAI harvester UA. It is live; a browser-only probe grades it dead.
- **OAI-PMH errors are HTTP 200.** Both providers return `<error code="...">` inside a 200 response. An agent grading on status code alone reads a rejected request as a success.
- Corrects the 2026-06-03 review, which recorded "SSO/IdP hosts did not resolve publicly" — the identity plane is at `shibboleth3.liv.ac.uk` and `fs.liverpool.ac.uk`, not `sso.liverpool.ac.uk`.
- `*.figshare.com` is wildcard DNS: `liverpool.figshare.com` resolves, and so does a nonsense subdomain. No Figshare tenancy is evidenced and none is recorded.
- No open data portal (`data.liverpool.ac.uk` does not resolve), no course/timetable API, and no `.well-known/security.txt`, `llms.txt` or `apis.json` on the main site.

## Maintainers

- Kin Lane — kin@apievangelist.com
