# DeSMòS Validation Report (v1.1.0 - Zenodo v2)

This file contains the documentation regarding the quality of the **DeSMòS** ontology, generated via the **OOPS! (OntOlogy Pitfall Scanner!)** tool.

## Evolution and Improvements (Preliminary Version vs. Version 1)

This validation refers to **Version 1.1.0** of the model. Compared to the preliminary **Version 1.0.0**, the refinement process has facilitated the elimination of several minor pitfalls, thereby consolidating the logical architecture and the interoperability of the `desmos:` namespace.

The iterative revision process has resulted in a substantial mitigation of the issues initially identified:
* **Resolution of Pitfall P08 (Missing Annotations)**: In version v1.0.0, 16 instances of missing annotations were detected for core elements such as `F1 Work`, `F2 Expression`, and `E39 Actor`. In version v1.1.0, this pitfall has been entirely eliminated.
* **Resolution of Pitfall P13 (Inverse Relationships)**: Version v1.0.0 presented 8 cases of inverse relationships that were not explicitly declared. In version v1.1.0, all necessary inverse properties have been implemented, resolving the issue in full.
* **Structural Consolidation**: The v1.1.0 model retains only those warnings related to the required interoperability with external standards, confirming the maturity and stability of the `desmos:` namespace.

## Results Summary (Version 1)

The automated analysis assigned the **"Minor Pitfalls"** conformance badge to the model. This indicates the absence of critical or important errors that could affect the ontology's consistency, reasoning, or applicability.
* **Pitfalls Detected**: 2 cases categorized as "Minor" importance.
* **Namespace Status**: 0 pitfalls detected for the original entities introduced by the model.
* **Suggestions**: 2 warnings regarding the potential definition of symmetric or transitive object properties.

## Justification of Residual Pitfalls

The "Minor" level pitfalls identified in the v1.1.0 report have been intentionally maintained to preserve alignment with international Cultural Heritage standards (**CIDOC CRM** and **LRMoo**):

* **P07 (Merging different concepts in the same class)**: Identified for the class `http://www.cidoc-crm.org/cidoc-crm/E29 Design or Procedure`. This is a **false positive** resulting from CIDOC CRM nomenclature; the conjunction "or" is an integral part of the official class name and does not indicate an improper merging of distinct concepts.
* **P22 (Using different naming conventions in the ontology)**: Flagged as a general "Minor" pitfall. This discrepancy arises from the necessary coexistence of the *CamelCase* convention adopted for DeSMòS and the alphanumeric/underscore notation of the CIDOC CRM standard (e.g., `E29_Design_or_Procedure`), which is essential for ensuring system interoperability.

---
*Validation performed on 15/04/2026.*