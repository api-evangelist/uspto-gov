# USPTO (uspto-gov)

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Patents
- Trademarks
- Intellectual Property
- Government
- Federal
- Open Data
- PTAB
- TSDR

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### USPTO Patent File Wrapper API

Core USPTO Open Data Portal (ODP) API for searching and retrieving U.S. patent application file wrappers — bibliographic data, assignment history, prosecution documents (office actions, responses, claims, drawings), continuity, foreign priority, attorney/agent info, and patent term adjustments. Replaces the legacy Patent Examination Data System (PEDS) and Patent Application Information Retrieval (PAIR). Requires an ODP API key. Data covers all publicly available U.S. patent applications from Patent Center.

- **Human URL:** [https://data.uspto.gov/apis/patent-file-wrapper/search](https://data.uspto.gov/apis/patent-file-wrapper/search)

#### Tags

- Patents
- File Wrapper
- Government
- Intellectual Property
- Open Data

#### Properties

- [Documentation](https://data.uspto.gov/apis/patent-file-wrapper/search)
- [Documentation](https://data.uspto.gov/apis/patent-file-wrapper/application-data)
- [Documentation](https://data.uspto.gov/apis/patent-file-wrapper/documents)
- [Documentation](https://data.uspto.gov/apis/patent-file-wrapper/assignments)
- [OpenAPI](openapi/uspto-patent-file-wrapper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-patent-file-wrapper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-patent-file-wrapper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/uspto-patent-application-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/uspto-gov-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### USPTO Patent Trial and Appeal Board (PTAB) API

Patent Trial and Appeal Board (PTAB) API v3 hosted on the Open Data Portal. 19 endpoints covering trial proceedings (IPR, PGR, CBM, derivation), trial decisions (institution, final written, terminations), trial documents (petitions, patent owner responses, expert declarations), and trial appeal/interference decisions. Coverage from 1997 to present; full PTAB Trial decisions and party briefing since September 2012. The legacy Developer Hub PTAB API was fully retired on January 6, 2026.

- **Human URL:** [https://developer.uspto.gov/api-catalog/ptab-api-v3-data-odp](https://developer.uspto.gov/api-catalog/ptab-api-v3-data-odp)

#### Tags

- PTAB
- Patents
- Trials
- Decisions
- Government
- Intellectual Property
- Open Data

#### Properties

- [Documentation](https://developer.uspto.gov/api-catalog/ptab-api-v3-data-odp)
- [Documentation](https://data.uspto.gov/apis/ptab-trials/search-documents)
- [Documentation](https://data.uspto.gov/apis/ptab-trials/search-decisions)
- [OpenAPI](openapi/uspto-ptab-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-ptab.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-ptab.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USPTO Trademark Status and Document Retrieval (TSDR) API

Trademark Status & Document Retrieval (TSDR) Data API — 24 endpoints (hosted on a separate server with a separate API key from the rest of ODP) for retrieving trademark case status, documents, and images by serial number, registration number, reference number, or international registration number. Returns case metadata in XML, JSON, and ST.96 formats and lets clients pull full file wrapper PDFs and ZIP packages. Rate limited at 60 requests/min/key for status calls and 4 requests/min/key for PDF/ZIP downloads.

- **Human URL:** [https://developer.uspto.gov/api-catalog/tsdr-data-api](https://developer.uspto.gov/api-catalog/tsdr-data-api)

#### Tags

- Trademarks
- TSDR
- Government
- Intellectual Property
- Document Retrieval
- Open Data

#### Properties

- [Documentation](https://developer.uspto.gov/api-catalog/tsdr-data-api)
- [Documentation](https://developer.uspto.gov/swagger/tsdr-api-v1)
- [Portal](https://tsdr.uspto.gov/)
- [Documentation](https://www.uspto.gov/sites/default/files/documents/tm-enterprise-api-user-guide-v2.pdf)
- [OpenAPI](openapi/uspto-tsdr-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-tsdr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-tsdr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/uspto-trademark-case-schema.json) — [JSON Schema](https://json-schema.org/specification)

### USPTO Office Action APIs

Family of 8 endpoints covering structured Office Action data — Text Retrieval, Citations, Rejections, and Enriched Citations. The Enriched Citation API uses machine-learning information extraction and entity resolution to normalize patent and non-patent literature citations against the application reference list. Office Action Weekly Archives are surfaced as bulk product OACT via SearchBulkProducts/GetBulkProduct. All legacy Office Action and Enriched Citation APIs were migrated to ODP ahead of the May 29, 2026 Developer Hub decommission.

- **Human URL:** [https://developer.uspto.gov/api-catalog/uspto-enriched-citation-api-v3](https://developer.uspto.gov/api-catalog/uspto-enriched-citation-api-v3)

#### Tags

- Patents
- Office Actions
- Citations
- Rejections
- Government
- Intellectual Property
- Machine Learning
- Open Data

#### Properties

- [Documentation](https://developer.uspto.gov/api-catalog/uspto-enriched-citation-api-v3)
- [Documentation](https://developer.uspto.gov/api-catalog/uspto-office-action-citations-api)
- [OpenAPI](openapi/uspto-office-actions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-office-actions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-office-actions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USPTO Bulk Data Storage System (BDSS) API

ODP Bulk Data API exposing the Bulk Data Storage System (BDSS) — SearchBulkProducts and GetBulkProduct operations for downloading patent and trademark bulk datasets (bibliographic, assignment, classification, office action weekly archives, etc.) as Entire Datasets (10-year increments) or Delta Datasets (daily increments) in XML/JSON. Methods support product lookup but do not allow general filter/limit/offset/order-by database queries.

- **Human URL:** [https://data.uspto.gov/apis/bulk-data/search](https://data.uspto.gov/apis/bulk-data/search)

#### Tags

- Bulk Data
- Patents
- Trademarks
- Datasets
- Government
- Open Data

#### Properties

- [Documentation](https://data.uspto.gov/apis/bulk-data/search)
- [Documentation](https://data.uspto.gov/apis/bulk-data/product)
- [Documentation](https://data.uspto.gov/patent-file-wrapper/bulkdata/entire)
- [Documentation](https://data.uspto.gov/documents/documents/BDSS-to-ODP-API-Mapping.pdf)
- [OpenAPI](openapi/uspto-bulk-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-bulk-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-bulk-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USPTO PatentsView API

USPTO research-oriented patent data API with inventor disambiguation, assignee, location, CPC/USPC classification, and citation endpoints. The database integrates the best available tools for inventor disambiguation and data quality control, supporting bibliometric and innovation research. PatentsView migrated into the USPTO Open Data Portal on March 20, 2026 — clients should obtain an ODP API key and use the ODP-hosted endpoints going forward.

- **Human URL:** [https://developer.uspto.gov/api-catalog/patentsview](https://developer.uspto.gov/api-catalog/patentsview)

#### Tags

- Patents
- Inventors
- Research
- Disambiguation
- Government
- Open Data

#### Properties

- [Documentation](https://developer.uspto.gov/api-catalog/patentsview)
- [Documentation](https://patentsview.org/apis/api-endpoints)
- [OpenAPI](openapi/uspto-patentsview-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uspto-patentsview.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uspto-patentsview.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.uspto.gov/)
- [Portal](https://data.uspto.gov/)
- [Documentation](https://developer.uspto.gov/api-catalog)
- [Documentation](https://data.uspto.gov/apis/getting-started)
- [Documentation](https://data.uspto.gov/apis/transition-guide)
- [Documentation](https://data.uspto.gov/documents/documents/BDSS-to-ODP-API-Mapping.pdf)
- [Documentation](https://www.uspto.gov/sites/default/files/documents/tm-enterprise-api-user-guide-v2.pdf)
- [Authentication](https://data.uspto.gov/apis/getting-started)
- [Rate Limits](https://developer.uspto.gov/files/tsdr-api-key-manager-user-guide)
- [Support](mailto:APIhelp@uspto.gov)
- [Support](mailto:contactUXD@uspto.gov)
- [Git Hub](https://github.com/USPTO)
- [Data Portal](https://catalog.data.gov/organization/uspto-gov)
- [Bulk Data](https://data.uspto.gov/patent-file-wrapper/bulkdata/entire)
- [Trademark](https://tsdr.uspto.gov/)
- [Trademark](https://www.uspto.gov/trademarks/apply/check-status-view-documents/trademark-bulk-data)
- [Patent](https://patentcenter.uspto.gov/)
- [Vocabulary](vocabulary/uspto-gov-vocabulary.yml)
- [Rate Limits](rate-limits/uspto-gov-rate-limits.yml)
