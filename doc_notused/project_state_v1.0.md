# Heritage Samples Registry Website — Project State

## Overview

The Heritage Samples Registry (HSR) website is at https://heritagesamples.org/ and is
built using Material for MkDocs. The source repository is at
https://github.com/HeritageSamples/heritagesamples.org. The site is deployed via GitHub

## Site structure

The site has two main navigation sections, About and Get Involved, plus a News page.

### About section

- **Home** — overview of the initiative with call-to-action buttons and a development
  status notice
- **About the Registry** — what the HSR is, why it exists, and how it fits into the
  broader landscape of E-RIHS, ECHOES, HSDS, and related projects
- **Key Definitions** — working definitions of Heritage Object, Heritage Fragment, and
  Heritage Sample, and their relationships
- **What is an IGSN?** — explanation of the IGSN identifier, its governance through
  IGSN e.V. and DataCite, resolvability, and a note clarifying the IGSN / IGSN ID
  terminology distinction
- **IGSNs in practice** — explains the four roles of the ecosystem once an IGSN is
  assigned: the Registry as PID authority, the IGSN in local systems, the
  human-readable destination for sample information, and DataCite Commons and the
  scholarly record; includes a summary table and sections on citing samples and
  resolvability
- **Goals & Scope** — core goals, what is in and out of scope, and future development
- **Project Team & Acknowledgements** — team members with ORCIDs, and funding
  acknowledgements for E-RIHS IP, ECHOES, HSDS/RICHeS, H-SEARCH, and NFDI4Objects

### Get Involved section

- **Consortium Vision** — long-term sustainability model, institutional pathways for
  minting IGSNs, governance, and international outlook
- **Who can benefit?** — audiences: heritage science institutions, researchers and
  conservators, collection and data managers, and contributors across the DOI/PID
  ecosystem
- **Using the Registry** — practical introduction to participation: when and how to
  register a sample, minimum and optional metadata requirements, how the IGSN
  integrates with local systems, metadata record submission, and resolvability
- **Register Your Interest** — two routes: email contact and a community survey
  (survey button present but currently disabled pending a live URL); includes who
  should register and what happens after
- **Roadmap** — phased development diagram rendered as a Mermaid flowchart

### News & Updates

- Single entry dated 2026-02-24 recording the initial draft website launch

## Technical setup

- Framework: Material for MkDocs
- Custom overrides directory: `overrides/`
- Custom footer in `overrides/partials/footer.html` — contains navigation links
  (About, Get Involved, Contact), copyright notice, and CC BY-NC 4.0 licence link
- Copyright year: 2026
- `generator: false` set in `mkdocs.yml` to suppress the default Material credit
- Custom CSS for disabled button styling (`.md-button--disabled`) to handle the
  inactive survey button on the Register Your Interest page
- Deployment via GitHub Actions on push to main branch

## Key design decisions and conventions

- The site uses "IGSN" throughout rather than "IGSN ID", with a brief explanatory note
  on the What is an IGSN? page acknowledging the formal DataCite term
- Em-dashes are not used anywhere on the site; commas or sentence recasting are used
  instead
- The Registry is consistently described as a PID authority and lightweight metadata
  record service, not a documentation repository or data store
- "Detailed analytical data", "conservation documentation", and similar are explicitly
  described as outside Registry scope, remaining in institutional systems
- The term "data" is used carefully throughout to avoid ambiguity: "metadata records"
  is used when referring to what the Registry holds; "data" is reserved for analytical
  or research content held elsewhere
- The disabled survey button uses a `span` element with class `md-button md-button--disabled`
  rather than an anchor tag, to avoid a dead link
- See Also sections use relative markdown paths; these should be checked against actual
  filenames if pages are renamed or moved

## Outstanding known issues

- The community survey button on Register Your Interest needs a live URL added once
  the survey is available; at that point the `span` element should be replaced with
  a standard markdown link button and the disabled class removed.

## Content principles

- British English throughout
- Professional and accessible tone; no marketing language or unsupported claims
- The service is consistently described as being in active development and pilot
  testing; claims about future capability are framed carefully
- No em-dashes
- Internal links use relative paths in markdown source; absolute URLs appear in
  rendered output

## Relationship to other work

The HSR website sits alongside the following related resources which may be referenced
in future sessions:

- Heritage Samples schema repository: https://github.com/HeritageSamples/schema
- IGSN e.V. website: https://ev.igsn.org/
- DataCite IGSN metadata guidance:
  https://support.datacite.org/docs/igsn-id-metadata-recommendations
- IGSN DataCite Archaeology and Cultural Heritage Community of Practice:
  https://ev.igsn.org/communities/archaeology
- ICCROM Register of Heritage Samples Archives: https://samplearchives.iccrom.org/
