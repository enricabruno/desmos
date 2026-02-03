# DeSMòS: Descriptive Semantic Model for Structured Texts

**DeSMòS** is an OWL ontology designed to model **literary constraints** as text-generating devices that shape the writing process and account for the genesis of specific textual forms

## 🎯 Project Objectives
The ontology provides a structured conceptual framework to describe:
* **Constraints as procedures**: constraints are modelled as generative mechanisms governing the writing process.
* **Conceptual origin**: a distinction between literary tradition and authorial invention, mediated through **SKOS-based controlled vocabularies**.
* **Scope of application**: the purpose of the constraint, distinguishing between the **formal** or **semantic** units to which the constraint is applied.
* **Evidence of identifiability**: mappings between textual features (**intratextual traces**) and authorial declarations (**paratextual** or **epitextual** statements).

## 🛠️ DeSMòS is aligned to international standards:

| Prefix | Standard | URI | 
| :--- | :--- | :--- |
| `crm` | **CIDOC CRM** | `http://www.cidoc-crm.org/cidoc-crm/` 
| `lrmoo` | **LRMoo** | `http://iflastandards.info/ns/lrm/lrmoo/`  
| `skos` | **SKOS** | `http://www.w3.org/2004/02/skos/core#` 
| `prov` | **PROV-O** | `http://www.w3.org/ns/prov#` 
| `dct` | **Dublin Core Terms** | `http://purl.org/dc/terms/` 

## 📁 Repository Structure
* **`/ontology`**: Contains the `desmos.ttl` (Turtle) and `desmos.owl` (RDF/XML) source files**
* **`/data`**: CSV tables containing the data collected for the case study, along with the corresponding mapping in RDF/Turtle.
* **`/queries`**: SPARQL queries used for functional validation and testing competency questions.
* **`/img`**: Graphical documentation of the **formal model**.
* **`/evaluation`**: Reports from **OOPS!** (OntOlogy Pitfall Scanner!) and consistency checks.

**Author:** Anonymous (Under review)  
**Version:** 1.0.1   **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 
