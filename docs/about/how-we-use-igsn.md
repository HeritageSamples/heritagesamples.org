# How we use IGSNs in the Heritage Samples Registry

The Heritage Samples Registry assigns **IGSNs (DOI-based persistent identifiers)** to physical samples so they can be **consistently referenced, discovered, and linked** to related research outputs over time.

An IGSN can be created **as soon as the minimum required descriptive information is available**. The Registry is **not a repository** for full datasets or detailed documentation: it provides a **stable identifier and a lightweight landing record**, with links out to information held elsewhere.

## When you can register a sample

You can register a sample and obtain an IGSN at any of these points:

- **At the time of sampling**, once the sample has been labelled and basic context recorded
- **At the time of creation**, if a sample is split or broken into parts and the new sample(s) has been labelled and basic context recorded
- **Retrospectively**, for legacy samples where the minimum information can be reconstructed
- **Before publication**, so the IGSN can be cited in reports, articles, and datasets

Registering early is encouraged. The record can be updated later as more documentation becomes available.

## What information is needed

The Registry aims to keep registration lightweight.

!!! note "Minimum information required"
    An IGSN can be assigned once the minimum descriptive metadata is available.  
    Detailed analytical data and documentation can remain in existing institutional systems.

### Minimum information (to create an IGSN record)

- A **local sample label or code** used by the custodian institution
- The **custodian** responsible for holding the sample
- A **source context** describing what the sample was taken from (an object identifier where available)
- The **person or organisation** responsible for creating/collecting/processing the sample
- A **publication date** for the registry record

### Optional information (recommended)

- A short **description of the sampling location** on the source
- A **link** that documents the sampling site (for example a IIIF resource or another persistent landing page)
- A **small representative image** (thumbnail) to support recognition and browsing
- Alternative or legacy identifiers already used locally
- Basic sample type and keywords
- Links to related outputs (datasets, publications, reports) as they become available

## Draft metadata model

The Registry is supported by a draft metadata model that defines the core information required to register and identify heritage science samples, together with a wider set of optional fields for richer description and linking. This model is being developed in alignment with IGSN and DataCite recommendations, while extending them to reflect the specific needs of heritage science research.

Initial versions of the draft schemas are being published openly as they are developed:
- [Heritage Samples draft schemas (GitHub)](https://github.com/HeritageSamples/schema)

These schemas are provided primarily for technical reference during the pilot phase. More detailed, user-oriented guidance on the metadata structure and its practical use will be added to this website as the pilot Registry service comes online.

## What the Registry stores (and what it doesn’t)

The Registry stores:

- The **IGSN / DOI**
- A **minimal descriptive record**
- Optional thumbnail image
- Links to external documentation and research outputs

The Registry does **not** store:

- Full analytical datasets
- Full-resolution images or extensive media collections
- Detailed institutional conservation documentation

Institutions retain their detailed documentation and datasets within their own systems. The Registry provides the persistent identifier and a lightweight landing record, and can list key links where useful; however, in the longer term these relationships are expected to be expressed and discovered through the broader DOI and PID infrastructure (for example via DataCite-related identifier links).

## Integration with existing systems

The Registry is designed to work alongside existing collection management systems, laboratory databases, and research repositories. Institutions do not need to replace their current documentation workflows or move their detailed data into the Registry.

Instead, local identifiers, records, and datasets can remain within institutional systems, while the Registry provides a persistent IGSN and a lightweight landing record that links outward to those existing resources. This approach supports interoperability and long-term discovery without duplicating or centralising detailed documentation.

## Linking samples to research outputs

Once an IGSN exists, it can be used as a stable reference point to connect a sample to:

- Publications and reports
- Datasets and repositories
- Project pages and catalogues
- Image-based documentation of sampling locations (including IIIF resources)

These links can be added and extended over time.

## Sample relationships (optional)

In many research workflows a sample may be subdivided, mounted, re-mounted, partially consumed, or otherwise processed. Where relevant, the Registry can capture simple relationships between samples (for example, a subsample derived from a parent sample) to support traceability over time.

---

**See also:**  
- [Goals & Scope](goals-scope.md)  
- [Register your interest](../get_involved/register-interest.md)
