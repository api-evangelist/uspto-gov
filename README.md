# USPTO (uspto-gov)

The United States Patent and Trademark Office (USPTO) is the federal agency that examines and grants U.S. patents and registers federal trademarks. Through its Open Data Portal (ODP) at **data.uspto.gov** and the legacy Developer Hub (developer.uspto.gov), USPTO publishes a tier-1 open-data API surface covering patent file wrappers, PTAB trial proceedings, office actions, enriched citations, bulk datasets, the long-running TSDR trademark API, and the research-focused PatentsView API (migrated to ODP in March 2026).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=government-api-evangelist&utm_content=repo)

## Tags

- Patents, Trademarks, Intellectual Property, Government, Federal, Open Data, PTAB, TSDR

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Migration Notes (2026)

- The legacy Developer Hub at `developer.uspto.gov` is being decommissioned on **May 29, 2026**; all APIs have moved to the Open Data Portal at `data.uspto.gov`.
- The Patent Examination Data System (PEDS) has been replaced by the **Patent File Wrapper API** on ODP.
- **PTAB API v2** was decommissioned on **January 6, 2026** in favor of **PTAB API v3** on ODP.
- **PatentsView** migrated to ODP on **March 20, 2026**.
- All ODP APIs require an **ODP API key**; TSDR uses a **separate** API key.

## APIs

### USPTO Patent File Wrapper API
Core ODP API for searching and retrieving U.S. patent application file wrappers — bibliographic data, assignments, prosecution documents, continuity, foreign priority, attorney/agent, and patent term adjustments. Replaces PEDS and PAIR.

**Human URL:** [https://data.uspto.gov/apis/patent-file-wrapper/search](https://data.uspto.gov/apis/patent-file-wrapper/search)

- [Documentation — Search](https://data.uspto.gov/apis/patent-file-wrapper/search)
- [Documentation — Application Data](https://data.uspto.gov/apis/patent-file-wrapper/application-data)
- [Documentation — Documents](https://data.uspto.gov/apis/patent-file-wrapper/documents)
- [Documentation — Assignments](https://data.uspto.gov/apis/patent-file-wrapper/assignments)
- [OpenAPI](openapi/uspto-patent-file-wrapper-openapi.yml)
- [JSON Schema — Patent Application](json-schema/uspto-patent-application-schema.json)
- [JSON-LD](json-ld/uspto-gov-context.jsonld)
- [Naftiko Capability — Patent File Wrapper](capabilities/patent-file-wrapper.yaml)

### USPTO Patent Trial and Appeal Board (PTAB) API
PTAB API v3 hosted on ODP. 19 endpoints covering trial proceedings (IPR, PGR, CBM, derivation), trial decisions, trial documents, appeals, and interferences. Coverage 1997 to present; full trial decisions since September 2012.

**Human URL:** [https://developer.uspto.gov/api-catalog/ptab-api-v3-data-odp](https://developer.uspto.gov/api-catalog/ptab-api-v3-data-odp)

- [Documentation — Search Documents](https://data.uspto.gov/apis/ptab-trials/search-documents)
- [Documentation — Search Decisions](https://data.uspto.gov/apis/ptab-trials/search-decisions)
- [OpenAPI](openapi/uspto-ptab-openapi.yml)
- [Naftiko Capability — PTAB Trials](capabilities/ptab-trials.yaml)

### USPTO Trademark Status and Document Retrieval (TSDR) API
24 endpoints (on a separate server with a separate API key) for retrieving trademark case status and file wrapper documents/images by serial number, registration number, reference number, or international registration number. Status in ST.66 XML, ST.96 XML, and JSON. Rate limits: 60 status calls/min/key and 4 PDF/ZIP downloads/min/key.

**Human URL:** [https://developer.uspto.gov/api-catalog/tsdr-data-api](https://developer.uspto.gov/api-catalog/tsdr-data-api)

- [Documentation — TSDR API v1 Syntax](https://developer.uspto.gov/swagger/tsdr-api-v1)
- [Documentation — TSDR API Key Manager User Guide](https://www.uspto.gov/sites/default/files/documents/tm-enterprise-api-user-guide-v2.pdf)
- [TSDR Web Portal](https://tsdr.uspto.gov/)
- [OpenAPI](openapi/uspto-tsdr-openapi.yml)
- [JSON Schema — Trademark Case](json-schema/uspto-trademark-case-schema.json)
- [Naftiko Capability — TSDR Status](capabilities/tsdr-status.yaml)
- [Naftiko Capability — TSDR Documents](capabilities/tsdr-documents.yaml)

### USPTO Office Action APIs
Family of 8 endpoints covering Text Retrieval, Citations, Rejections, and Enriched Citations. The Enriched Citation API uses machine-learning information extraction and entity resolution to normalize patent and non-patent literature citations against the application's reference list.

**Human URL:** [https://developer.uspto.gov/api-catalog/uspto-enriched-citation-api-v3](https://developer.uspto.gov/api-catalog/uspto-enriched-citation-api-v3)

- [OpenAPI](openapi/uspto-office-actions-openapi.yml)
- [Naftiko Capability — Office Actions](capabilities/office-actions.yaml)

### USPTO Bulk Data Storage System (BDSS) API
ODP Bulk Data API exposing SearchBulkProducts and GetBulkProduct over patent and trademark bulk datasets (bibliographic, assignment, classification, office-action weekly archives) as Entire Datasets (10-year increments) or Delta Datasets (daily increments).

**Human URL:** [https://data.uspto.gov/apis/bulk-data/search](https://data.uspto.gov/apis/bulk-data/search)

- [Documentation — Product Data](https://data.uspto.gov/apis/bulk-data/product)
- [Documentation — BDSS to ODP Mapping (PDF)](https://data.uspto.gov/documents/documents/BDSS-to-ODP-API-Mapping.pdf)
- [OpenAPI](openapi/uspto-bulk-data-openapi.yml)
- [Naftiko Capability — Bulk Data](capabilities/bulk-data.yaml)

### USPTO PatentsView API
Research-focused patent data API with inventor disambiguation, assignee, location, CPC/USPC classification, and citation endpoints. Migrated into the USPTO Open Data Portal on March 20, 2026.

**Human URL:** [https://developer.uspto.gov/api-catalog/patentsview](https://developer.uspto.gov/api-catalog/patentsview)

- [OpenAPI](openapi/uspto-patentsview-openapi.yml)

## Common Resources

- [Website](https://www.uspto.gov/)
- [Open Data Portal](https://data.uspto.gov/)
- [API Catalog](https://developer.uspto.gov/api-catalog)
- [ODP Getting Started](https://data.uspto.gov/apis/getting-started)
- [PEDS to ODP Transition Guide](https://data.uspto.gov/apis/transition-guide)
- [GitHub Organization](https://github.com/USPTO)
- [Catalog on data.gov](https://catalog.data.gov/organization/uspto-gov)
- [Patent Center](https://patentcenter.uspto.gov/)
- [Trademark Bulk Data](https://www.uspto.gov/trademarks/apply/check-status-view-documents/trademark-bulk-data)
- [Vocabulary](vocabulary/uspto-gov-vocabulary.yml)
- [Rate Limits](rate-limits/uspto-gov-rate-limits.yml)

## Support

- API help: APIhelp@uspto.gov
- Developer/UX support: contactUXD@uspto.gov
