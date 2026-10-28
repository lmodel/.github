# lmodel

LinkML models of published specifications, standards and vocabularies. lmodel is a workshop for LinkML patterns: no model here is an official release of what it renders, and most have no users yet. Each model's address, `https://w3id.org/lmodel/<repository>`, redirects to its documentation site.

## What a usable model has

A host can pin a usable model, adapt it for its knowledge bundle and import it. [slsa](https://github.com/lmodel/slsa) is the reference for every item.

- A [linkml-project-copier](https://github.com/linkml/linkml-project-copier) project at template v0.5.0, or, in a fork of an upstream project, the same toolchain beside the upstream's code. The CONTRIBUTING checklist, the SECURITY policy, the code of conduct, the AI covenant, NOTICE, and lint configuration for links, Markdown, YAML and LinkML.
- A schema header with the upstream's edition in `version`, its canonical address in `source`, and the licence. An upstream watch pinned to that edition reports when it moves.
- A copy of the upstream text only where its licence allows, matched to the edition by hash, and a citation by address and date otherwise.
- A valid example for each class a concept may name as its type, a counter-example for each constraint the schema states, tests green, and `linkml-lint` clean under the repository's `.linkmllint.yaml`.
- Semantic-release from a baseline tag. Each GitHub release carries `schema-<tag>-<name>.yaml`, its `.sha256` and a build-provenance attestation.
- A [KTL](https://w3id.org/ktl/) sidecar at the current KTL release with lokf 0.9.0 or later, a librarian-written knowledge bundle and a knowledge website. `just lokf-adapt` with named roots, `just lokf-adapt-check` in CI, and a README section listing the classes for the *Known LOKF types* setting and the keys the copy renames.
- A README that says what the schema models and at which edition, what shaped its design, and what it maps to without borrowing from.
- PyPI publishing off until a consumer needs the Python classes.
- A row below.

## Repositories

The waves bring each repository to the list above, one repository at a time. A new repository joins when a host needs its classes as concept types or two models need it as a shared import, and it has a stable, licensed, machine-readable source to pin. The `version` column is the schema header's as it stands.

### Wave 0: the reference

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [slsa](https://github.com/lmodel/slsa) | SLSA specification; the reference | 1.2.0 | v0.6.0 |
| [gist](https://github.com/lmodel/gist) | gist, the Semantic Arts upper ontology | 14.1.0 | v0.5.0 |

### Wave 1: the evidence set

The models a supply-chain knowledge bundle cites as authorities: the workflow contract, the attestation container, assessment results, the SBOM and the secure development practices.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| github-actions (new) | GitHub Actions workflow syntax, action metadata and repository rulesets | | |
| in-toto (new) | in-toto Attestation Framework | | |
| [oscal](https://github.com/lmodel/oscal) | OSCAL | 1.2.1 | |
| [spdx](https://github.com/lmodel/spdx) | SPDX | 3.0.1 | |
| [nist-sp-800-218](https://github.com/lmodel/nist-sp-800-218) | NIST SP 800-218, Secure Software Development Framework | 1.1.0 | |

### Wave 2: the controls set

Control catalogues, with `oscal` as their pivot.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [nist-sp-800-53](https://github.com/lmodel/nist-sp-800-53) | NIST SP 800-53 Rev. 5 controls and SP 800-53A assessment procedures | 5.2.0 | |
| [nist-sp-800-171](https://github.com/lmodel/nist-sp-800-171) | NIST SP 800-171 Rev. 3 | 3.0.0 | |
| [nist-csf-v2](https://github.com/lmodel/nist-csf-v2) | NIST Cybersecurity Framework 2.0 | 2.0.0 | |
| [cis-controls](https://github.com/lmodel/cis-controls) | CIS Controls | 8.1.2 | |
| [iso27001](https://github.com/lmodel/iso27001) | ISO/IEC 27001 | 1.0.0 | |

### Wave 3: the threat and case set

`attack` follows `stix`, whose schema it carries. The Unified Cyber Ontology repositories become one repository, `uco`, with a module for each, and each module keeps its address.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [stix](https://github.com/lmodel/stix) | STIX 2.1 | | |
| [attack](https://github.com/lmodel/attack) | MITRE ATT&CK | | |
| uco-action, uco-analysis, uco-configuration, uco-core, uco-identity, uco-location, uco-marking, uco-master, uco-observable, uco-pattern, uco-role, uco-time, uco-tool, uco-types, uco-victim, uco-vocabulary | Unified Cyber Ontology | 1.1.0 | |

### Wave 4: the vocabularies

`ucs-core` and `ucs-containers`, a use-case framework with no upstream, are archived until a model needs them.

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [collections](https://github.com/lmodel/collections) | Collections Ontology | 2.0.0 | |
| [void](https://github.com/lmodel/void) | VoID | | |
| [datatype](https://github.com/lmodel/datatype) | AGLDWG Datatype Ontology | 1.0 | |

### Wave 5: the vulnerability set

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

### Wave 6: the AI governance and privacy set

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

### Wave 7: the finance set

| Repository | Models | `version` | Release |
| --- | --- | --- | --- |
| [fix-protocol](https://github.com/lmodel/fix-protocol) | FIX Protocol | | |
| [fix-orchestra](https://github.com/lmodel/fix-orchestra) | FIX Orchestra | 1.1-rc2 | |
| [fix-sbe](https://github.com/lmodel/fix-sbe) | FIX Simple Binary Encoding | | |
| [fixp](https://github.com/lmodel/fixp) | FIX Performance Session Protocol | FIX.5.0SP2 | |
| [common-domain-model](https://github.com/lmodel/common-domain-model) | FINOS Common Domain Model, in a fork | | |
| [calm](https://github.com/lmodel/calm) | FINOS Common Architecture Language Model, in a fork | 1.2 | |
| [fluxnova-bpm-platform](https://github.com/lmodel/fluxnova-bpm-platform) | FINOS Fluxnova BPM Platform, in a fork | 2.0.0-SNAPSHOT | |

### Wave 8: the agent tooling set

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
