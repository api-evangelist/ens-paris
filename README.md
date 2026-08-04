# École Normale Supérieure de Paris (ens-paris)

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

École Normale Supérieure de Paris (ENS, rue d'Ulm) is a leading French grande école and constituent member of Université PSL (Paris Sciences & Lettres), ranked #86 in the QS World University Rankings 2025. This repository catalogs the institution's public developer/API footprint as an [APIs.json](https://apisjson.org) profile.

- APIs.json: <https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/apis.yml>
- Run with Naftiko: <https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=ens-paris-api-evangelist&utm_content=repo>

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, Open Access, France

## APIs

ENS Paris does not publish a first-party developer portal or documented institutional API. The programmatic surface relevant to ENS is reached through national French research and open-data infrastructure:

- **HAL-ENS Open Archive (OAI-PMH)** — ENS researcher output deposited in HAL, harvestable via the national HAL OAI-PMH server. Docs: <https://api.archives-ouvertes.fr/docs/oai>
- **HAL Search / REST API** — query publication metadata including HAL-ENS records. Docs: <https://api.hal.science/docs/>
- **MESR Higher Education Open Data (Explore API)** — French Ministry open-data platform exposing ENS establishment/enrolment data (third-party). Docs: <https://data.enseignementsup-recherche.gouv.fr/api/explore/v2.1/console>

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/ens-paris-plans-pricing.yml](plans/ens-paris-plans-pricing.yml)
- Rate Limits: [rate-limits/ens-paris-rate-limits.yml](rate-limits/ens-paris-rate-limits.yml)
- FinOps: [finops/ens-paris-finops.yml](finops/ens-paris-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: <https://www.ens.psl.eu/en>
- LinkedIn: <https://www.linkedin.com/school/ecole-normale-superieure/>
- Plans, Rate Limits, FinOps, Review (see files above and [review.yml](review.yml))

## Notes

All endpoints in this profile were probed live on 2026-06-03; no endpoints were fabricated. ENS itself exposes no documented developer API — the cataloged APIs are national/third-party platforms (HAL, MESR open data) that carry ENS-relevant data. No official ENS Paris GitHub organization exists at `github.com/ens-paris` (HTTP 404). The LinkedIn school page is included by standard slug; LinkedIn returns HTTP 999 to automated fetchers, so it was not directly retrievable.

## Maintainers

- Kin Lane — kin@apievangelist.com
