# Open Charge Map (api-evangelist-openchargemap)

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

Open Charge Map is the global public registry of electric vehicle charging locations, established in 2011 as a non-commercial, community-driven project. The platform maintains a crowdsourced dataset of 300,000+ charging points worldwide, combining manually entered data with imported open data from government registries and charging networks. The REST API enables developers to search and retrieve POI (Points of Interest) data on EV charging stations, including location details, equipment specifications, connection types, operator information, and user-submitted check-ins and photos. Data can be filtered by geographic coordinates, bounding box, country, operator, connection type, charging level, and operational status. The API is free to use with an API key registration and supports both read (GET) and write (POST) operations for contributing new charging location data.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/openchargemap/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/openchargemap/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Electric Vehicles
- EV Charging
- Charging Stations
- Points of Interest
- Open Data
- Geospatial
- Transportation
- Clean Energy
- Crowdsourced
- Registry

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Open Charge Map POI API

Primary REST API for searching and retrieving EV charging station data (Points of Interest) from the Open Charge Map global registry. Supports geographic search by latitude/longitude with distance radius, bounding box filtering, country filtering, and filtering by operator, connection type, charging level, usage type, and operational status. Returns full POI data including address, equipment details, connection types, power levels, operator info, and user comments. Supports compact and verbose output formats in JSON. An API key is required and passed as a query parameter or HTTP header.

- **Human URL:** [https://openchargemap.org/site/develop/api](https://openchargemap.org/site/develop/api)
- **Base URL:** `https://api.openchargemap.io/v3`

#### Tags

- EV Charging
- Points of Interest
- Geospatial Search
- Charging Stations

#### Properties

- [Documentation](https://openchargemap.org/site/develop/api)
- [Git Hub](https://github.com/openchargemap/ocm-system)

### Open Charge Map Reference Data API

REST API endpoint returning core reference data used for interpreting POI results, including connection types, charging levels, operators, countries, status types, usage types, supply types (AC/DC), and submission status types. This data provides the lookup tables needed to decode numeric ID fields returned in POI results. Can be filtered by country. Returns reference data in JSON format with an API key.

- **Human URL:** [https://openchargemap.org/site/develop/api](https://openchargemap.org/site/develop/api)
- **Base URL:** `https://api.openchargemap.io/v3`

#### Tags

- Reference Data
- Connection Types
- Operators
- Countries

#### Properties

- [Documentation](https://openchargemap.org/site/develop/api)

### Open Charge Map POI Submit API

REST API endpoint for contributing new EV charging station data or updating existing POI records in the Open Charge Map global registry. Requires an authenticated API key associated with a registered Open Charge Map user account. Submitted data is reviewed and integrated into the community dataset. Supports adding new charging locations with full address, equipment, connection type, and operator details.

- **Human URL:** [https://openchargemap.org/site/develop/api](https://openchargemap.org/site/develop/api)
- **Base URL:** `https://api.openchargemap.io/v3`

#### Tags

- Submit
- Contribute
- Crowdsourced
- Data Entry

#### Properties

- [Documentation](https://openchargemap.org/site/develop/api)

## Common Properties

- [Website](https://openchargemap.org/)
- [Documentation](https://openchargemap.org/site/develop/api)
- [Developer](https://openchargemap.org/site/develop)
- [Git Hub](https://github.com/openchargemap/ocm-system)
- [Git Hub Org](https://github.com/openchargemap)
- [Community](https://community.openchargemap.org/)
- [Apps](https://openchargemap.org/site/develop/apps)
- [Terms of Service](https://openchargemap.org/site/about/terms)
- [About](https://openchargemap.org/site/about)
- [Plans](plans/openchargemap-plans.yml)
- [Rate Limits](rate-limits/openchargemap-rate-limits.yml)
- [Fin Ops](finops/openchargemap-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
