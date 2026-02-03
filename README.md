# DeSMòS: Descriptive Semantic Model for Structured texts

**DeSMòS** is an OWL ontology designed to represent **literary constraints** as generative engines that drive writing process and determine the genesis of specific textual forms.

## 🎯 Project Objectives
The ontology provides a structured conceptual framework to describe:
* **Constraints as procedures**: Modeled as generative action plans, following the `E29_Design_or_Procedure` class.
* **Conceptual origin**: Distinction between literary tradition and authorial invention, mediated by **SKOS** controlled vocabularies.
* **Evidence of identifiability**: Mapping between **textual features** (intratextual traces) and **authorial declarations** (paratextual or epitextual statements).

## 🛠️ DeSMòS is aligned to international standards:

| Prefix | Standard | URI |
| :--- | :--- | :--- | :--- |
| `crm` | **CIDOC CRM** | `http://www.cidoc-crm.org/cidoc-crm/` 
| `lrmoo` | **LRMoo** | `http://iflastandards.info/ns/lrm/lrmoo/`  
| `skos` | **SKOS** | `http://www.w3.org/2004/02/skos/core#` 
| `prov` | **PROV-O** | `http://www.w3.org/ns/prov#` 
| `dct` | **Dublin Core** | `http://purl.org/dc/terms/` 

## 📁 Repository Structure
* **`/ontology`**: Contains the `desmos.ttl` (Turtle) and `desmos.owl` (RDF/XML) source files**
* **`/data`**: The **Oplepiana** dataset from *La Biblioteca Oplepiana* (in riga edizioni, 2005).
* **`/queries`**: SPARQL queries used for functional validation and testing competency questions.
* **`/img`**: Graphical documentation of the **formal model**.
* **`/evaluation`**: Reports from **OOPS!** (OntOlogy Pitfall Scanner!) and consistency checks.

**Author:** Anonymous (Under review)  
**Version:** 1.0.1   **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 
