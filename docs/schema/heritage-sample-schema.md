# Heritage Sample Schema

This page provides an early technical overview of the schema used by the
**Heritage Samples Registry** for assigning IGSNs and managing core metadata.

!!! info "Draft status"
    The schema described here is a **working draft** and will evolve as the
    Registry develops and the consortium expands.

---

## 1. Purpose

The Heritage Sample Schema is designed to:

- ensure every registered sample can receive a valid **IGSN–DOI**,  
- capture the **minimal, internationally consistent metadata** required
  for cross-institution discovery,
- preserve alignment with domain-specific local systems  
  (e.g., paintings, archaeological objects, geological collections).

---

## 2. JSON Schema (excerpt)

=== "JSON Schema"

    ```json
    {
      "$id": "https://heritagesamples.org/schema/heritage-sample-v0.1.json",
      "$schema": "https://json-schema.org/draft/2020-12/schema",
      "title": "Heritage Sample",
      "description": "Minimal profile for registering IGSN-compliant heritage samples.",
      "type": "object",
      "required": ["sampleId", "creator", "sampleType", "sampleOrigin"],
      "properties": {
        "sampleId": {
          "type": "string",
          "description": "Local institutional sample identifier or code."
        },
        "creator": {
          "type": "string",
          "description": "Institution or lab responsible for sample creation or extraction."
        },
        "sampleType": {
          "type": "string",
          "description": "High-level sample type (e.g., paint cross-section, textile fibre)."
        },
        "sampleOrigin": {
          "type": "object",
          "required": ["label"],
          "properties": {
            "label": {
              "type": "string",
              "description": "Human-readable label for the original object."
            },
            "pid": {
              "type": "string",
              "format": "uri",
              "description": "Persistent identifier for the source object (if available)."
            }
          }
        }
      }
    }
    ```

=== "Example record"

    ```json
    {
      "sampleId": "IRPA-PS-2025-012",
      "creator": "KIK-IRPA",
      "sampleType": "paint cross-section",
      "sampleOrigin": {
        "label": "Portrait of an Unknown Lady",
        "pid": "https://example.org/object/1234"
      }
    }
    ```

---

## 3. How this schema fits into the Registry

```mermaid
graph TD
    A[Local Sample Record<br/>IRPA-PS-2025-012] -->|registered in| B[Heritage Samples Registry]
    A -->|assigned| C[IGSN-DOI]
    B -->|exposes| D[Public Metadata]
    D -->|links to| E[Institutional Systems]
