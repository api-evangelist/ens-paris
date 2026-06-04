# École Normale Supérieure de Paris (ens-paris)

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
