# Rithum

Rithum is a commerce operations platform providing dropship, marketplace, and supply chain integration solutions for retailers, brands, and suppliers. Formerly known as CommerceHub and ChannelAdvisor, Rithum connects brands and retailers to manage product listings, inventory, order workflows, and performance across ecommerce channels. The platform powers the Dsco API for dropship and marketplace integrations. In 2025, Rithum launched RithumIQ, an AI engine for automated commerce recommendations and operational insights.

**Website:** [https://www.rithum.com](https://www.rithum.com)

**Documentation:** [https://api.dsco.io/doc/v3/reference/](https://api.dsco.io/doc/v3/reference/)

## APIs

### Dsco Platform API

The Dsco Platform API v3 provides dropship and marketplace commerce integration for retailers and suppliers. It supports order management, catalog synchronization, inventory updates, shipment tracking, returns processing, and invoice workflows via streaming and batch endpoints. Authentication uses OAuth2 bearer tokens.

- **Base URL:** `https://api.dsco.io/api/v3`
- **Authentication:** OAuth2 Bearer Token
- **Documentation:** [https://api.dsco.io/doc/v3/reference/](https://api.dsco.io/doc/v3/reference/)
- **Getting Started:** [https://knowledge.rithum.com/s/article/Getting-started-with-the-Rithum-V3-API](https://knowledge.rithum.com/s/article/Getting-started-with-the-Rithum-V3-API)

#### Key Capabilities

- **Order Management** — Retailer order creation and supplier order retrieval
- **Catalog Synchronization** — Supplier product catalog creation and updates
- **Inventory Updates** — Real-time inventory quantity management
- **Shipment Tracking** — Shipment record creation with tracking numbers
- **Returns Processing** — Return creation and completion workflows
- **Invoice Workflows** — Invoice submission for fulfilled orders
- **Event Streaming** — Near-real-time event delivery via partitioned streams

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [openapi/dsco-platform-openapi.yml](openapi/dsco-platform-openapi.yml) | Dsco Platform API v3 — orders, catalog, inventory, shipments, returns, invoices, streams |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [rules/dsco-platform-rules.yml](rules/dsco-platform-rules.yml) | Dsco API linting rules enforcing camelCase operationIds, batch request patterns, and bearer auth |

### Capabilities

| Capability | Description |
|------------|-------------|
| [capabilities/commerce-operations.yaml](capabilities/commerce-operations.yaml) | Unified workflow for dropship/marketplace commerce operations |
| [capabilities/shared/dsco-platform.yaml](capabilities/shared/dsco-platform.yaml) | Shared Dsco Platform API consumed definition |

### JSON Schemas

| Schema | Description |
|--------|-------------|
| [json-schema/dsco-order-schema.json](json-schema/dsco-order-schema.json) | Dsco platform order with line items and shipping address |
| [json-schema/dsco-catalog-item-schema.json](json-schema/dsco-catalog-item-schema.json) | Dsco product catalog item with SKU, cost, and retail model rules |

### JSON Structure

| Structure | Description |
|-----------|-------------|
| [json-structure/dsco-order-structure.json](json-structure/dsco-order-structure.json) | Field-by-field documentation of the order object |

### JSON-LD Context

| Context | Description |
|---------|-------------|
| [json-ld/rithum-context.jsonld](json-ld/rithum-context.jsonld) | Linked data context mapping Rithum/Dsco terms to schema.org |

### Examples

| Example | Description |
|---------|-------------|
| [examples/dsco-supplier-list-orders-example.json](examples/dsco-supplier-list-orders-example.json) | List supplier orders with request/response |
| [examples/dsco-supplier-create-shipment-example.json](examples/dsco-supplier-create-shipment-example.json) | Create a shipment record with tracking |

### Vocabulary

| Vocabulary | Description |
|------------|-------------|
| [vocabulary/rithum-vocabulary.yml](vocabulary/rithum-vocabulary.yml) | Commerce domain terms including Dropship, Marketplace, Order, Stream, SKU |

## Tags

Commerce, Dropship, Marketplace, Ecommerce, Supply Chain, Retail

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
