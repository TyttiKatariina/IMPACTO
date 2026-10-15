# IMPACTO
**Impact Assessment Ontology (IMPACTO)**
An ontology for impact assessments under the GDPR and the EU AI Act: Data
Protection Impact Assessments (DPIA, GDPR Art. 35) and Fundamental Rights
Impact Assessments (FRIA, AI Act Art. 27).

Documentation: [https://tyttikatariina.github.io/IMPACTO/](https://tyttikatariina.github.io/IMPACTO/). 

Namespace: `https://tyttikatariina.github.io/IMPACTO/#`
Prefix: `impacto`

**Contact:**
This ontology is created and maintained by:
Tytti Rintamäki
PhD Candidate
ADAPT Centre, Dublin City University, Dublin, Ireland
tytti.rintamaki@adaptcentre.ie
GitHub: tyttikatariina

## The ontology

| File | Format |
|---|---|
| [impacto.ttl](impacto.ttl) | Turtle |
| [impacto.rdf](impacto.rdf) | RDF/XML |
| [impacto.jsonld](impacto.jsonld) | JSON-LD |

## Contents

| Path | What it is |
|---|---|
| `impacto.*` | The ontology |
| `information-requirements.ttl` | The information each assessment must contain, from GDPR Art. 35(7) and AI Act Art. 27(1) |
| `proposed-concepts.ttl` | Concepts proposed to DPV |
| `conditions/DPIAConditions.ttl` | 995 conditions under which a DPIA is required (114 Conditions in total but divided by each jurisdiction, the amount climbs to 995) |
| `conditions/DPIANotRequiredConditions.ttl` | 80 conditions under which no DPIA is required (66 Conditions in total but divided by each jurisdiction, the amount climbs to 80) |
| `conditions/FRIAConditions.ttl` | Conditions under which a FRIA is required, and the Annex III processing patterns |
| `competency-questions/` | The competency questions and the queries answering them |
| `dpia-sparql/`, `fria-sparql/` | Queries by topic |
| `dpia-shacl/` | SHACL shapes |
| `usecase/` | Three worked deployments |
| `example.ttl` | A worked example |

## Scope

IMPACTO represents:

- **when each assessment is required**, including the variation between Member
  States — the conditions come from GDPR Art. 35 and from the Art. 35(4) and
  35(5) lists published by 30 supervisory authorities
- **what each assessment must contain**, from GDPR Art. 35(7) and AI Act
  Art. 27(1)(a)–(f)
- **how the two overlap**: which high-risk processing activities are carried
  out through high-risk AI systems, and which deployments owe both assessments
- **what a FRIA may reuse from a DPIA** under AI Act Art. 27(4), and what each
  reused element does not cover

The FRIA obligation is narrower than the high-risk classification: a system may
be high-risk under Art. 6(2) and still owe no FRIA, depending on the category
of deployer. IMPACTO keeps the two apart.

## Built on

The [Data Privacy Vocabulary](https://w3id.org/dpv) 2.3 and its GDPR, AI Act
and fundamental rights extensions. Terms carry the name of the DPV module they
are proposed for as part of their local name, so
`impacto:eu-gdpr-DPIARequiredProcess` is proposed for the `eu-gdpr` extension.

## Citation

Pending

## Licence

[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
