# Cargolux (cargolux)

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
