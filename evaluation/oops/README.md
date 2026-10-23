# OOPS! evaluation of DeSMòS

- Tool: OOPS! (OntOlogy Pitfall Scanner!)
- Ontology: `data/ontology/desmos.owl` (version 1.2.0)
- Date: 2026-10-23
- Report: see the PDF in this folder

## Remaining pitfalls

| Pitfall | Importance | Assessment |
|---|---|---|
| P07 Merging different concepts in the same class | Minor | Lexical trigger on "or" in the reused CIDOC CRM class `E29_Design_or_Procedure`, whose official definition is unitary. |
| P11 Missing domain or range | Important | Affects only reused properties (`skos:inScheme`, `dcterms:created`, `dcterms:issued`, `schema:pagination`, `intro:R44_hasWording`) whose official specifications do not declare them. All DeSMòS properties declare both. |
| P13 Inverse relationships not declared | Minor | `skos:inScheme` and `prov:wasAttributedTo` have no inverse defined in SKOS or PROV-O. All DeSMòS object properties declare an inverse. |
| P22 Different naming conventions | Minor | Caused by reused vocabularies (CIDOC CRM, LRMoo, INTRO use underscores). DeSMòS uses UpperCamelCase for classes and lowerCamelCase for properties. |

The suggestion on symmetric/transitive properties is not applied to P130, R76 and skos:broader/narrower, which the official specifications define as non-transitive.

No critical pitfalls were detected.