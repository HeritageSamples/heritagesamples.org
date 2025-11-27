# About the Heritage Samples Registry

<img style="float: right" hspace="20" width="128px" src="../../images/hs-logo_v1.3-dark.png"/>

The **Heritage Sample Registry (HSR)** is a collaborative initiative to create a sustainable and interoperable registry for heritage samples, built on the [**International Generic Sample Number (IGSN)**](https://ev.igsn.org/) system. Each IGSN is a [**Digital Object Identifier (DOI)**](https://www.doi.org/), providing a persistent, globally resolvable reference that connects physical samples to the international DOI network and supports reliable cross-referencing in publications and data resources. 

Developed within the framework of [**E-RIHS (European Research Infrastructure for Heritage Science)**](https://www.e-rihs.eu/), the work draws on developments begun under [**IPERION HS**](https://www.iperionhs.eu/) and is now supported through [**ECHOES**](https://www.echoes-eccch.eu/) and [**RICHeS**](https://www.riches.ukri.org/). The HSR will provide a common mechanism for the identification and citation of physical heritage samples, beginning with **paint cross-sections**. Each sample will be assigned a unique IGSN and a minimal descriptive record, enabling it to be referenced unambiguously across multiple systems and publications. 

The registry will form the foundation for **digital twin representations** of heritage samples, providing a persistent link between the physical sample and its digital surrogates, including analytical data and related documentation held elsewhere.

```mermaid
---
config:
  layout: fixed
---
flowchart LR
    A@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/sample_vial.jpg\" width=\"64\"><br>Physical Heritage Sample" } --> HSR@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/hs-logo_v1.3-dark.png\" width=\"72\"><br>Heritage Samples Registry<br>IGSN–DOI Assignment" }
    HSR --> B@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/metadata-card.png\" width=\"64\"><br>Minimal Core Metadata Record" } & IGSN@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/igsn.jpg\" width=\"64\"><br>IGSN-DOI Identifier" }
    IGSN --> DOI@{ label: "<img src=\"https://upload.wikimedia.org/wikipedia/commons/1/11/DOI_logo.svg\" width=\"64\"><br>DOI Infrastructure" }
    B --> IGSN
    C@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/data.png\" width=\"64\"><br>External Data<br>Images, Analysis, Documentation" } -. references .-> IGSN
    D@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/publications.png\" width=\"64\"><br>Publications &amp; Reports" } -. references .-> IGSN
    E@{ label: "<img src=\"https://heritagesamples.github.io/heritagesamples.org/images/DigitalTwin.png\" width=\"64\"><br>Digital Twin Representations" } -. references .-> IGSN
    C -. may also have .-> DOI
    D -. may also have .-> DOI
    E -. may also have .-> DOI

    A@{ shape: rect}
    HSR@{ shape: rect}
    B@{ shape: rect}
    IGSN@{ shape: rect}
    DOI@{ shape: rect}
    C@{ shape: rect}
    D@{ shape: rect}
    E@{ shape: rect}
     A:::object
     HSR:::digital2
     B:::dims2
     IGSN:::name2
     DOI:::digital2
     C:::infoobj
     D:::document
     E:::infoobj
    classDef object stroke:#2C5D98,fill:#2C5D98,color:#FFFFFF,rx:5px,ry:5px,font-size:18px,font-weight:bold
    classDef digital2 stroke:#999,fill:#eee,color:black,rx:5px,ry:5px,font-size:18px,font-weight:bold
    classDef name2 stroke:orange,fill:#FEF3BA,color:black,rx:20px,ry:20px,font-size:18px,font-weight:bold
    classDef infoobj stroke:#907010,fill:#fffa40,color:black,rx:20px,ry:20px,font-size:18px,font-weight:bold
    classDef document stroke:#2C5D98,fill:#33B0FF,color:#2C5D98,rx:5px,ry:5px,font-size:18px,font-weight:bold
    classDef dims2 stroke:black,fill:#c6c6c6,color:black,rx:20px,ry:20px,font-size:18px,font-weight:bold
```

## **Purpose and Rationale** 

Heritage science increasingly depends on access to data from small but significant physical samples that are analysed, reused, and reinterpreted across institutions and decades of research. Despite their importance, these samples often lack consistent public identifiers, making it difficult to trace their provenance, usage, or analytical history. 

The HSR addresses this problem by: 

- Assigning a **persistent IGSN-DOI** to each sample, ensuring long-term traceability and interoperability. 

- Providing a **shared metadata structure** aligned with the default IGSN and DataCite schemas, with limited heritage-specific extensions (such as sample location on an object or sample type). 

- Supporting the creation of **digital twins**, linking physical samples to their related digital resources in external systems. 

- Offering a **federated registry** that allows institutions to register and manage identifiers locally while contributing to an international reference index. 

- Enabling connections to institutional collection management systems and open research repositories through standard APIs and linked data practices. 

It is important to emphasise that the registry will not host analytical results, publications, or detailed documentation. Its sole function is to provide authoritative identifiers and core metadata to support interoperability across the broader digital ecosystem of heritage science. 

## Acknowledgement
This project was setup as part of the work of the following projects:

### The Horizon Europe [E-RIHS IP](https://www.e-rihs.eu/the-project/) project
[<img width="256px" src="https://e-rihs.io/graphics/e-rihs-eric-logo_ai.png" alt="E-RIHS IP Logo">](https://www.e-rihs.eu)<br/>
* [E-RIHS IP has received funding from the European Union’s Horizon Europe call HORIZON-INFRA-2021-DEV-02, Grant Agreement n.101079148.](https://cordis.europa.eu/project/id/101079148)

### The Horizon Europe [ECHOES](https://www.echoes-eccch.eu/) project
[<img width="256px" src="https://www.echoes-eccch.eu/wp-content/uploads/2024/07/ECHOES_Logo.png" alt="ECHOES Logo">](https://www.echoes-eccch.eu/)<br/>
* [ECHOES is a project funded by the European Commission under Grant Agreement n.101157364 – ECHOES.](https://cordis.europa.eu/project/id/101157364)
* [ECHOES is a project funded by UK Research and Innovation (UKRI) under the UK government’s Horizon Europe funding guarantee n.10110142 & n.10110466.]()

### The [UKRI RICHeS](https://www.riches.ukri.org/) [HSDS](https://hsds.ac.uk/) project
[<img width="256px" src="https://hsds.ac.uk/wp-content/uploads/2024/09/HSDS_Blue-and-black_1920px.png" alt="HSDS Logo">](https://hsds.ac.uk/)<br/>
* [HSDS is a project funded by UK Research and Innovation (UKRI) as part of the RICHeS Programme.](https://www.riches.ukri.org/)

### The [H-SEARCH](https://rdm.kikirpa.be/projects/h-search/) project
[<img width="256px" src="https://rdm.kikirpa.be/wp-content/uploads/2025/01/H-SEARCH-colour-logo.png" alt="H-SEARCH Logo">](https://rdm.kikirpa.be/projects/h-search/)<br/>
* [H-SEARCH is a project funded by the Belgian Science Policy Office (BELSPO) as part of the IMPULS INFRA Programme, grant number IM/RT/23/H-SEARCH.](https://www.belspo.be/)
