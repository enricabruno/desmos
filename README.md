# DeSMòS: Descriptive Semantic Model for Structured texts

**DeSMòS** is an OWL ontology designed to represent **literary constraints** as generative engines that drive the writing process and determine the genesis of specific textual forms.

## 🎯 Project Objectives
The ontology provides a structured conceptual framework to describe:
* **Constraint as procedure**: Modeled as generative engine, following the `E29_Design_or_Procedure` class.
* **Conceptual origin**: Distinction between literary tradition and oulipian invention, mediated by **SKOS** controlled vocabularies.
* **Evidence of identifiability**: Mapping between **textual features** (objective intratextual traces detectable in the lrmoo:F2_Expression) and the constraints they reveal.
* **Constraint Declaration**: Formal representation of **paratextual** or **epitextual statements** where the constraint is explicitly named or described. Following the removal of a dedicated class, these declarations are now modelled as crm:E33_Linguistic_Object instances directly linked to the rule they describe via the crm:P129_is_about property, enabling streamlined verification of authorial intent.

## 🛠️ DeSMòS is aligned to international standards:

| Prefix | Standard | URI | 
| :--- | :--- | :--- |
| `crm` | **CIDOC CRM** | `http://www.cidoc-crm.org/cidoc-crm/` 
| `lrmoo` | **LRMoo** | `http://iflastandards.info/ns/lrm/lrmoo/`  
| `skos` | **SKOS** | `http://www.w3.org/2004/02/skos/core#` 
| `prov` | **PROV-O** | `http://www.w3.org/ns/prov#` 
| `dcterms` | **Dublin Core** | `http://purl.org/dc/terms/` 

## 📁 Repository Structure
* **`/ontology`**: Contains the `desmos.owl` (RDF/XML) source file**
* **`/data`**: The **Oplepiana** dataset from *La Biblioteca Oplepiana* (in riga edizioni, 2005).
* **`/img`**: Graphical documentation of the **formal model**.
* **`/OOPSevaluation`**: Reports from **OOPS!** (OntOlogy Pitfall Scanner!) and consistency checks.

**Author:** Enrica Bruno
**Version:** 1.1.0   **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 
