# Attio (attio-com)

Attio is an AI-native customer relationship management (CRM) platform built on a flexible object/attribute/record data model. The Attio REST API (base `https://api.attio.com/v2`) exposes that data model programmatically - objects, records, attributes, lists, list entries, notes, tasks, comments, threads, workspace members, and webhooks - letting teams sync data, build workflows, and extend the CRM. Requests are authenticated with a Bearer access token (API key or OAuth 2.0) and scoped by granular permissions.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/apis.yml)

## Tags

- CRM
- Customer Relationship Management
- AI
- Sales
- Data Model
- Objects and Records

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Attio Objects API

List, create, get, and update the objects (people, companies, deals, users, workspaces, and custom objects) that define the schema of an Attio workspace. Objects are the top-level model that records and attributes hang off of.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/objects/list-objects](https://docs.attio.com/rest-api/endpoint-reference/objects/list-objects)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Objects
- Data Model
- Schema

#### Properties

- [Documentation](https://docs.attio.com/rest-api/how-to/data-model)
- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/objects/list-objects)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Records API

Full lifecycle for records within any object - query (list with filter and sort), create, get, update (append or overwrite multiselect values), delete, and assert/upsert by a matching attribute. Also lists a record's attribute value history and the list entries a record belongs to.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/records/list-records](https://docs.attio.com/rest-api/endpoint-reference/records/list-records)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Records
- CRUD
- Upsert

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/records/list-records)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Attributes API

Manage the attributes (typed fields) defined on an object or a list - list, create, get, and update attributes, plus manage the select options and statuses that power select-type and status-type attributes.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/attributes/list-attributes](https://docs.attio.com/rest-api/endpoint-reference/attributes/list-attributes)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Attributes
- Schema
- Select Options

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/attributes/list-attributes)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Lists API

Create, list, get, and update lists - the collections that model a specific process (such as a sales pipeline) by referencing records from one or more objects and layering their own attributes on top.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/lists/list-all-lists](https://docs.attio.com/rest-api/endpoint-reference/lists/list-all-lists)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Lists
- Pipelines
- Views

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/lists/list-all-lists)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio List Entries API

Manage the entries within a list - query (filter and sort), add a record as a new entry, get, update (append or overwrite multiselect values), delete, and assert/upsert an entry by its parent record, plus read entry-specific attribute values.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/entries/list-entries](https://docs.attio.com/rest-api/endpoint-reference/entries/list-entries)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- List Entries
- Pipelines
- CRUD

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/entries/list-entries)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Deals API

The Deals CRM surface, expressed through the standard records endpoints with the object set to `deals` - query, create, get, update, delete, and upsert deal records with value, stage, and associated people and companies.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/deals/list-deals](https://docs.attio.com/rest-api/endpoint-reference/deals/list-deals)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Deals
- Sales
- Pipeline

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/deals/list-deals)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Notes API

Create, list, get, and delete notes attached to records - free-form plaintext or Markdown content used to capture context and activity against a person, company, deal, or other record.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/notes/list-notes](https://docs.attio.com/rest-api/endpoint-reference/notes/list-notes)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Notes
- Activity
- CRM

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/notes/list-notes)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Tasks API

Create, list, get, update, and delete tasks - actionable to-dos with a deadline, completion status, assignees, and links to the records they relate to.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/tasks/list-tasks](https://docs.attio.com/rest-api/endpoint-reference/tasks/list-tasks)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Tasks
- Workflow
- Assignments

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/tasks/list-tasks)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Comments and Threads API

Collaboration on records and list entries. List and get threads of comments, and create, get, and delete individual comments within a thread, record, or entry - the discussion layer of the CRM.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/threads/list-threads](https://docs.attio.com/rest-api/endpoint-reference/threads/list-threads)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Comments
- Threads
- Collaboration

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/threads/list-threads)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Webhooks API

Create, list, get, update, and delete webhooks and their event subscriptions. Attio delivers HMAC-SHA256-signed HTTP POST callbacks to your target URL when records, list entries, notes, tasks, and comments change.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/webhooks/list-webhooks](https://docs.attio.com/rest-api/endpoint-reference/webhooks/list-webhooks)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Webhooks
- Events
- Subscriptions

#### Properties

- [Documentation](https://docs.attio.com/rest-api/guides/webhooks)
- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/webhooks/list-webhooks)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Workspace Members API

List and get the workspace members - the human users that belong to an Attio workspace - used to resolve assignees, note authors, and access controls.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/workspace-members/list-workspace-members](https://docs.attio.com/rest-api/endpoint-reference/workspace-members/list-workspace-members)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Workspace Members
- Users
- Identity

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/workspace-members/list-workspace-members)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Attio Meta / Self API

Identify the current access token - the workspace it is linked to, the authorizing member, and the scopes and permissions it holds. Useful for token introspection and health checks before making other calls.

- **Human URL:** [https://docs.attio.com/rest-api/endpoint-reference/meta/identify](https://docs.attio.com/rest-api/endpoint-reference/meta/identify)
- **Base URL:** `https://api.attio.com/v2`

#### Tags

- Meta
- Self
- Token Introspection

#### Properties

- [API Reference](https://docs.attio.com/rest-api/endpoint-reference/meta/identify)
- [OpenAPI](openapi/attio-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/attio-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/attio-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/attio)
- [LinkedIn](https://www.linkedin.com/company/attio)
- [Website](https://attio.com/)
- [Documentation](https://docs.attio.com/)
- [Plans](plans/attio-com-plans-pricing.yml)
- [Rate Limits](rate-limits/attio-com-rate-limits.yml)
- [Fin Ops](finops/attio-com-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
