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

École Normale Supérieure de Paris (ENS, rue d'Ulm) is a leading French grande école and constituent member of Université PSL (Paris Sciences & Lettres), ranked #86 in the QS World University Rankings 2025. This repository catalogs the institution's public developer/API footprint as an [APIs.json](https://apisjson.org) profile.

- APIs.json: <https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/apis.yml>
- Run with Naftiko: <https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=ens-paris-api-evangelist&utm_content=repo>

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

University, Higher Education, Education, France, Université PSL, Research, Identity Federation, Library, Open Access, OAI-PMH

## APIs

ENS-PSL publishes no developer portal, no OpenAPI description and no API key programme. It does
operate two machine-readable surfaces on its own domain, and holds one tenant relationship on a
national platform. All three were probed live on 2026-08-30.

- **ENS-PSL Identity Provider (SAML 2.0 / Shibboleth)** — *operator: institution*. SAML entity
  descriptor at <https://federation.ens.psl.eu/idp/shibboleth> (HTTP 200, `application/xml`),
  registered in the RENATER Fédération Éducation-Recherche with `shibmd:Scope` `ens.fr` and
  `ens.psl.eu`.
- **ENS-PSL Library Catalogue (Koha REST + OAI-PMH)** — *operator: institution*. Unauthenticated
  REST routes under <https://catalogue.bib.ens.psl.eu/api/v1/public/>, browsable at
  <https://catalogue.bib.ens.psl.eu/api/v1/.html>; OAI-PMH 2.0 provider at
  <https://catalogue.bib.ens.psl.eu/cgi-bin/koha/oai.pl?verb=Identify>, identifying as
  "bibliothèques de l'ENS-PSL". The interface contract is Koha's, so no OpenAPI is stored here.
- **HAL-ENS Open Archive, ENS-PARIS collection** — *operator: tenant*. ENS deposits inside the
  national HAL archive run by CCSD/CNRS; harvestable as OAI-PMH set `collection:ENS-PARIS`, and
  84,784 records are returned by HAL's ENS-scoped Search API. Docs:
  <https://api.archives-ouvertes.fr/docs/oai>

### Removed on 2026-08-30 — vendor contract, not ENS's

Two OpenAPI definitions previously in this repository described the **Opendatasoft Explore API
v2.1** running on the French Ministry of Higher Education portal
`data.enseignementsup-recherche.gouv.fr` — `info.contact: support@opendatasoft.com`, license
"Copyright Opendatasoft". ENS neither operates that portal nor is a tenant of it; it is a record
inside someone else's dataset. Both specs, the pre-refine original, and every schema, structure,
example, ruleset, agentic-access profile and collection derived from them were removed.

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/ens-paris-plans-pricing.yml](plans/ens-paris-plans-pricing.yml)
- Rate Limits: [rate-limits/ens-paris-rate-limits.yml](rate-limits/ens-paris-rate-limits.yml)
- FinOps: [finops/ens-paris-finops.yml](finops/ens-paris-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-08-30

## Common Properties

- Website: <https://www.ens.psl.eu/en>
- Legal notice / terms: <https://www.ens.psl.eu/mentions-legales>
- News RSS: <https://www.ens.psl.eu/en/rss.xml>
- Identity federation: <https://federation.ens.psl.eu/idp/shibboleth>
- Library catalogue: <https://catalogue.bib.ens.psl.eu/>
- Research repository: <https://hal-ens.archives-ouvertes.fr/>
- LinkedIn: <https://www.linkedin.com/school/ecole-normale-superieure/>
- Conformance: [conformance/ens-paris-conformance.yml](conformance/ens-paris-conformance.yml)
- Authentication: [authentication/ens-paris-authentication.yml](authentication/ens-paris-authentication.yml)
- Plans, Rate Limits, FinOps, Review (see files above and [review.yml](review.yml))

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles **who operates
each surface** before saving anything. Every endpoint in this profile was probed live; none was
fabricated.

- ENS publishes no `llms.txt` (404), no `/jsonapi` or `/api` on the main site (404), and nothing
  answers at `api.`, `data.`, `developer.`, `opendata.`, `git.` or `gitlab.` under `ens.psl.eu`.
- No official ENS Paris GitHub organization was found (`github.com/ens-paris`, `github.com/ENSPSL`,
  `github.com/ENS-Paris` all 404).
- **No ENS Figshare tenancy exists.** `ens.figshare.com` and `ens-psl.figshare.com` return the same
  empty HTTP 202 as a nonsense subdomain, so the host is a wildcard, not evidence of a tenancy.
- `moodle.ens.psl.eu` is a live institution-hosted Moodle with a SAML service provider registered in
  RENATER, but every LTI path probed redirects to the site home, so no LTI conformance is claimed.
- The library OAI-PMH provider advertises a baseURL of `/opac/oai.pl` that returns 404 from outside;
  the working base is `/cgi-bin/koha/oai.pl`.
- The LinkedIn school page returns HTTP 999 to automated fetchers — a bot block, not a dead link.
- ENS-PSL Kin Score conformance hits under the `education` regime: `saml`, `shibboleth` and
  `oai-pmh` (institution-operated), plus `oai-pmh` via the HAL tenancy. See
  [conformance/ens-paris-conformance.yml](conformance/ens-paris-conformance.yml).

## Maintainers

- Kin Lane — kin@apievangelist.com
