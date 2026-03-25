# IGSNs in practice

When the Heritage Samples Registry assigns an IGSN to a sample, it does more than create
a label. The identifier becomes part of a shared, global infrastructure that connects
physical samples to the wider ecosystem of scholarly research, across institutions,
systems, and time.

This page explains the roles that the Registry, the IGSN itself, and the broader
persistent identifier (PID) infrastructure each play once an identifier has been assigned.

## The Registry as PID authority

The Registry's primary function is to act as the authoritative source for each IGSN it
assigns. It holds the definitive record for that identifier: which institution registered
the sample, who holds it, and when the record was created. This record is what external 
systems and users can rely on as the definitive point of reference for that identifier.

The Registry is not primarily a browsing interface for sample information. In normal
operation it will be accessed directly by systems, such as collection management platforms,
laboratory databases, and other research infrastructure, rather than by researchers
navigating to it in a browser. Its core role is to make the identifier reliable and
machine-readable.

That said, the Registry is intended to provide simple search and navigation pages so that
users can explore what samples are registered and discover whether similar material
already exists in the system. This discovery function is secondary to its role as a PID
authority, but it is a valued part of the service.

Because each IGSN is implemented as a DOI, it takes the form of a resolvable URL. Anyone
who follows that link, from a citation in a publication, a reference in a dataset, or a
record in an external system, will be taken directly to the Registry's landing record
for that sample. This is what makes the identifier genuinely actionable rather than simply
a label, and it is the mechanism through which the Registry connects the physical sample
to the broader ecosystem described in the sections below.

## The IGSN in local systems

Once an IGSN has been assigned, institutions will typically continue to use their existing
human-readable labels and local identifiers as the primary means of referring to a sample
within their own systems. The IGSN is recorded alongside these as a persistent alternative
identifier, providing a stable, globally resolvable reference that connects the local
record to the wider research infrastructure.

Beyond simply storing the IGSN, it is important that the identifier propagates into any
documentation, reporting, or data outputs associated with the sample. When a sample is
described in an analytical report, referenced in a dataset, or cited in a publication, the
IGSN should be included so that the sample can be unambiguously identified and traced by
others. This is what transforms the identifier from an internal record into a meaningful
part of the scholarly record.

## Citing and referencing samples

One of the most significant benefits of assigning an IGSN is the ability to cite a
physical sample with the same precision and permanence that a DOI provides for a
publication or dataset. Once a sample has an IGSN, it can be referenced in journal
articles, technical reports, and published datasets in a way that is unambiguous and
persistent over time.

Researchers can include an IGSN citation in their methods sections, supplementary data,
or reference lists, allowing readers to identify exactly which physical material was
studied. This supports reproducibility, enables future researchers to identify and 
potentially seek access to the same sample, and creates a traceable connection between 
the physical sample and the research outputs it has contributed to.

## The human-readable destination for sample information

Detailed information about a sample, such as its analytical history, associated images,
and conservation documentation, is held and presented wherever the institution or project
chooses to make it publicly accessible. The Registry record carries a direct link to that
destination, so that anyone resolving the IGSN can be directed to a fuller presentation
of the sample and its associated information.

This destination will often be a page maintained by the holding institution, but it may
equally be an external platform or service. Data repositories, aggregators, and
infrastructure services such as the Heritage Science Data Service (HSDS), the Museum Data
Service, or Art UK could all serve as the human-readable home for sample information,
depending on the institution and sample type. The Registry itself does not reproduce or
host that content; it provides the persistent link to wherever it lives.

## DataCite Commons and the scholarly record

Each IGSN assigned through the Registry is submitted to DataCite as a DOI, entering the
same global infrastructure used to register publications, datasets, and other research
outputs. Through DataCite Commons, connections can be made between a sample's IGSN and
the publications or datasets that reference it, creating a navigable record of how a
sample has been used in research over time.

This is where the long-term value of persistent identification becomes most visible. A
sample taken decades ago and referenced across multiple publications can, with an IGSN,
become a traceable node in the scholarly record rather than an ambiguous local reference.
Over time, as more research outputs include IGSN citations, this network of connections
grows, making the contributions of physical samples to heritage science progressively
more visible and discoverable.

## Summary: four roles, one identifier

| Role | Provided by |
|---|---|
| PID authority and definitive source | The Heritage Samples Registry |
| Persistent identifier in local and external systems | The IGSN, recorded alongside institutional identifiers |
| Human-readable destination for sample information | The holding institution, or an external platform or repository |
| Connection to publications, datasets, and the scholarly record | DataCite Commons and the wider DOI infrastructure |

---

**See also:**

- [About the Registry](../about/about-registry.md)
- [What is an IGSN?](../about/what-is-igsn.md)
- [Using the Registry](../get_involved/using-the-registry.md)
