# lmodel

LinkML models of published specifications, standards and vocabularies. A workshop for LinkML patterns, all unofficial. Each model's address, `https://w3id.org/lmodel/<repository>`, redirects to documentation.

## What a usable model has

A project can pin a usable model, and adapt.

The pattern is a [linkml-project-copier](https://github.com/linkml/linkml-project-copier) project (or sidecar), with same CONTRIBUTING, SECURITY, CODE_OF_CONDUCT, AI_COVENANT, NOTICE, lint configuration, and Semantic-release. Each GitHub release carries `schema-<tag>-<name>.yaml` with provenance.

A [KTL](https://w3id.org/ktl/) sidecar, a librarian-written knowledge bundle and a knowledge website. Domain schema are [adapted](https://lokf.nolan-nichols.com/toolkit/adapt/), and [slsa](https://github.com/lmodel/slsa) is the reference.

## Repositories

A new repository joins as needed.

### Reference

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [slsa](https://github.com/lmodel/slsa) | SLSA specification; the reference | 1.2.0 | [v0.10.0](https://github.com/lmodel/slsa/releases/tag/v0.10.0) |
| [gist](https://github.com/lmodel/gist) | gist, the Semantic Arts upper ontology | 14.1.0 | [v0.7.0](https://github.com/lmodel/gist/releases/tag/v0.7.0) |

### Evidence

The models a supply-chain knowledge bundle cites as authorities:  workflow contract, attestation container, assessment results, SBOM and secure development practices.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [github-actions](https://github.com/lmodel/github-actions) | GitHub Actions workflow syntax, action metadata and repository rulesets | 2026-10-28 | [v0.5.0](https://github.com/lmodel/github-actions/releases/tag/v0.5.0) |
| [in-toto](https://github.com/lmodel/in-toto) | in-toto Attestation Framework: statement layer and vetted predicates | 1.2.0 | [v0.3.0](https://github.com/lmodel/in-toto/releases/tag/v0.3.0) |
| [oscal](https://github.com/lmodel/oscal) | Open Security Controls Assessment Language (OSCAL) | 1.2.3 | [v0.1.2](https://github.com/lmodel/oscal/releases/tag/v0.1.2) |
| [spdx](https://github.com/lmodel/spdx) | SPDX | 3.0.1 | [v0.1.0](https://github.com/lmodel/spdx/releases/tag/v0.1.0) |
| [nist-sp-800-218](https://github.com/lmodel/nist-sp-800-218) | NIST SP 800-218, Secure Software Development Framework | 1.1.0 | [v0.1.1](https://github.com/lmodel/nist-sp-800-218/releases/tag/v0.1.1) |

### Controls

Control catalogues, with `oscal` as their pivot.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [nist-sp-800-53](https://github.com/lmodel/nist-sp-800-53) | NIST SP 800-53 Rev. 5 controls and SP 800-53A assessment procedures | 5.2.0 | [v0.1.0](https://github.com/lmodel/nist-sp-800-53/releases/tag/v0.1.0) |
| [nist-sp-800-171](https://github.com/lmodel/nist-sp-800-171) | NIST SP 800-171 Rev. 3 | 3.0.0 | [v0.1.0](https://github.com/lmodel/nist-sp-800-171/releases/tag/v0.1.0) |
| [nist-csf-v2](https://github.com/lmodel/nist-csf-v2) | NIST Cybersecurity Framework 2.0 | 2.0.0 | [v0.1.0](https://github.com/lmodel/nist-csf-v2/releases/tag/v0.1.0) |
| [cis-controls](https://github.com/lmodel/cis-controls) | CIS Controls | 8.1.2 | [v0.2.0](https://github.com/lmodel/cis-controls/releases/tag/v0.2.0) |
| [iso27001](https://github.com/lmodel/iso27001) | ISO/IEC 27001 | 2022/Amd 1:2024 | [v0.1.0](https://github.com/lmodel/iso27001/releases/tag/v0.1.0) |

### Threat and Case

`attack` follows `stix`, whose schema it carries. `uco` has a module for each part of the Unified Cyber Ontology.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [stix](https://github.com/lmodel/stix) | STIX 2.1 | 2.1 | [v0.1.0](https://github.com/lmodel/stix/releases/tag/v0.1.0) |
| [attack](https://github.com/lmodel/attack) | MITRE ATT&CK | 20.0 | [v0.1.0](https://github.com/lmodel/attack/releases/tag/v0.1.0) |
| [uco](https://github.com/lmodel/uco) | Unified Cyber Ontology | 1.5.0 | [v0.3.0](https://github.com/lmodel/uco/releases/tag/v0.3.0) |

### Vocabularies

`ucs-core` and `ucs-containers`, a use-case framework with no upstream, are archived until a model needs them.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [collections](https://github.com/lmodel/collections) | Collections Ontology | 2.0 | [v0.2.0](https://github.com/lmodel/collections/releases/tag/v0.2.0) |
| [void](https://github.com/lmodel/void) | VoID | 2011-03-03 | [v0.1.0](https://github.com/lmodel/void/releases/tag/v0.1.0) |
| [datatype](https://github.com/lmodel/datatype) | AGLDWG Datatype Ontology | 2019-10-03 | [v0.1.0](https://github.com/lmodel/datatype/releases/tag/v0.1.0) |

### Vulnerability

`vulnerability-core` goes first, because `cve`, `nist-nvd` and `kev-catalog` import it.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [vulnerability-core](https://github.com/lmodel/vulnerability-core) | A shared base for vulnerability records | 1.0.0 | |
| [cve](https://github.com/lmodel/cve) | CVE Record Format | 5.2.0 | |
| [nist-nvd](https://github.com/lmodel/nist-nvd) | NIST National Vulnerability Database feeds | | |
| [kev-catalog](https://github.com/lmodel/kev-catalog) | CISA Known Exploited Vulnerabilities Catalog | 1.0 | |
| [cwe](https://github.com/lmodel/cwe) | CWE | 7.3 | |
| [capec](https://github.com/lmodel/capec) | CAPEC | | |
| [d3fend](https://github.com/lmodel/d3fend) | MITRE D3FEND | | |
| [ocsf](https://github.com/lmodel/ocsf) | Open Cybersecurity Schema Framework | 1.9.0-dev | |

### AI governance and Privacy

`nist-ai-600-1` and `nist-ai-rmf` import `nist-ai-100-1`, so the three go in that order.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [nist-ai-100-1](https://github.com/lmodel/nist-ai-100-1) | NIST AI 100-1, AI Risk Management Framework 1.0 | 1.0.0 | |
| [nist-ai-600-1](https://github.com/lmodel/nist-ai-600-1) | NIST AI 600-1, Generative AI Profile | 1.0.0 | |
| [nist-ai-rmf](https://github.com/lmodel/nist-ai-rmf) | NIST AI 100-1 and AI 600-1 together | 1.0.0 | |
| [iso42001](https://github.com/lmodel/iso42001) | ISO/IEC 42001 | 1.0.0 | |
| [iso22989](https://github.com/lmodel/iso22989) | ISO/IEC 22989 | 0.1.0 | |
| [iso29100](https://github.com/lmodel/iso29100) | ISO/IEC 29100 | 1.0.0 | |
| [dpv](https://github.com/lmodel/dpv) | Data Privacy Vocabulary | 2.3 | |
| [ai-governance-framework](https://github.com/lmodel/ai-governance-framework) | FINOS AI Governance Framework, in a fork | 0.1.0 | |

### Finance

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [fix-protocol](https://github.com/lmodel/fix-protocol) | FIX Protocol | | |
| [fix-orchestra](https://github.com/lmodel/fix-orchestra) | FIX Orchestra | 1.1-rc2 | |
| [fix-sbe](https://github.com/lmodel/fix-sbe) | FIX Simple Binary Encoding | | |
| [fixp](https://github.com/lmodel/fixp) | FIX Performance Session Protocol | FIX.5.0SP2 | |
| [common-domain-model](https://github.com/lmodel/common-domain-model) | FINOS Common Domain Model, in a fork | | |
| [calm](https://github.com/lmodel/calm) | FINOS Common Architecture Language Model, in a fork | 1.2 | |
| [fluxnova-bpm-platform](https://github.com/lmodel/fluxnova-bpm-platform) | FINOS Fluxnova BPM Platform, in a fork | 2.0.0-SNAPSHOT | |

### Agent tooling

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [mcp](https://github.com/lmodel/mcp) | Model Context Protocol | draft | |
| [dspy](https://github.com/lmodel/dspy) | DSPy | 0.1.0 | |
| [opa](https://github.com/lmodel/opa) | Open Policy Agent, in a fork | 0.1.0 | |
| [mellea](https://github.com/lmodel/mellea) | Mellea, in a fork | 2026-05-26 | |

### Not models

- [linkml-project-copier](https://github.com/lmodel/linkml-project-copier): a fork of the LinkML project template.
- [sssom-files](https://github.com/lmodel/sssom-files): mapping files in the SSSOM TSV format.
- [w3id_smoke_test](https://github.com/lmodel/w3id_smoke_test): tests the `w3id.org/lmodel` redirects.
