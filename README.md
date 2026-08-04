# Cargolux (cargolux)

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

Cargolux Airlines International S.A. is Europe's largest all-cargo airline, headquartered at Luxembourg Findel Airport in Luxembourg and operating a global Boeing 747 freighter network under IATA designator CV and air waybill prefix 172 (with Cargolux Italia on prefix 356). In the logistics chain Cargolux is the main-leg air carrier: it sells capacity to freight forwarders and general sales agents rather than to shippers, hands cargo to terminal and ground handling operators such as its Luxcargo Handling subsidiary, and files customs and security data on behalf of the contracted forwarder. Its API posture is honestly a customer-contract one. Cargolux publishes no developer portal and no machine-readable contract of any kind — developer.cargolux.com, developers.cargolux.com and docs.cargolux.com do not resolve, and /developers, /api, /openapi.json, /swagger.json, /api-docs and /.well-known/ all return 404 on www.cargolux.com. The only public self-service surfaces are HTML: a track-and-trace widget and a flight scheduler on the marketing site, plus a login-walled Customer Portal at my.cargolux.com. A real quote-and-booking API exists, but it is a bilateral, commercially negotiated forwarder interface — piloted with Kuehne+Nagel in 2021 and extended to DB Schenker — with no published reference, and it is complemented by indirect distribution through the cargo.one, CargoAi and WebCargo by Freightos marketplaces. Underneath, Cargolux runs IBS Software's iCargo SaaS cargo management system and holds a large minority stake in Luxembourg's CHAMP Cargosystems, whose developer.champ.aero portal is the developer surface Cargolux's ecosystem actually reads — CHAMP's, not Cargolux's. IATA e-AWB "Single Process" is documented; no IATA ONE Record or Cargo-XML publication was found.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cargolux/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cargolux/refs/heads/main/apis.yml)

## Tags

- Logistics
- Supply Chain
- Luxembourg
- Air Cargo
- Airlines
- Freight
- Track and Trace
- Standards

## Timestamps

- **Created:** 2026-07-30
- **Modified:** 2026-07-30

## APIs

No publicly documented APIs. Every developer-convention path was probed on 2026-07-30 and
returned 404 or failed DNS resolution. `apis[]` in `apis.yml` is intentionally empty — see
[review.yml](review.yml) for the full probe log, HTTP statuses and the interoperability
assessment.

## Interoperability

| Dimension | Finding |
| --- | --- |
| Standard conformance | IATA e-AWB / "Single Process" claimed in prose only; Cargo-IMP FSU status vocabulary observed in the public tracker payload; no ONE Record and no Cargo-XML publication found |
| Interface shape | `proprietary-undocumented` |
| Identifier scheme | IATA air waybill numbers (prefixes 172 / 356 + 8-digit serial), airline designator CV, IATA airport codes and flight numbers |
| Event model | `none-published` |
| EDI legacy | e-AWB documented in prose; Cargo-IMP FSU codes observed; no EDIFACT / X12 / AS2 / VAN onboarding published |
| Multi-party posture | Contracted forwarders and GSAs only; direct API is bilateral and per-forwarder; open access delegated to cargo.one, CargoAi and WebCargo by Freightos |
| Access gate | `commercial-agreement` |

## Common Properties

- [Website](https://www.cargolux.com/)
- [Customer Portal](https://my.cargolux.com/)
- [Customer Service](https://www.cargolux.com/customer-service/)
- [Your Shipment's Journey](https://www.cargolux.com/your-shipment-s-journey/)
- [Track and Trace](https://www.cargolux.com/track-and-trace/)
- [Flight Scheduler](https://www.cargolux.com/flight-scheduler/)
- [Go Paperless (e-AWB)](https://www.cargolux.com/your-shipment-s-journey/go-paperless/)
- [Terms of Use](https://www.cargolux.com/terms-of-use/)
- [Conditions of Carriage](https://www.cargolux.com/conditions-of-carriage/)
- [Conditions of Contract](https://www.cargolux.com/conditions-of-contract/)
- [General Terms and Conditions of Cargo Sales](https://www.cargolux.com/general-terms-and-conditions-of-cargo-sales/)
- [Data Protection](https://www.cargolux.com/data-protection/)
- [Cookie Policy](https://www.cargolux.com/cookie-policy/)
- [Media Releases](https://www.cargolux.com/media/media-releases/)
- [LinkedIn](https://www.linkedin.com/company/cargolux-airlines/)
- [Facebook](https://www.facebook.com/CargoluxAirlines)
- [Twitter](https://twitter.com/Cargolux_Intl)
- [GitHub Organization](https://github.com/cargolux)
- [Contact](https://www.cargolux.com/contact/)

## Maintainers

- Kin Lane — kin@apievangelist.com
