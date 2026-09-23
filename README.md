# DeSMòS: Descriptive Semantic Model for Structured Texts

**DeSMòS** is an OWL 2 ontology designed to represent **literary constraints** as generative procedures that guide the writing process and contribute to the genesis of specific textual forms.

## 🎯 Project Objectives

The ontology provides a structured conceptual framework to describe:

* **Constraint as procedure**: modeled as a generative procedure, following the `crm:E29_Design_or_Procedure` class.
* **Conceptual origin**: distinction between literary tradition and Oulipian invention, mediated by **SKOS** controlled vocabularies.
* **Evidence of identifiability**: mapping between **textual features** (intratextual traces detectable in an `lrmoo:F2_Expression`) and the constraints they reveal.
* **Constraint declaration**: representation of **paratextual** or **epitextual statements** in which a constraint is explicitly named or described. These declarations are modeled as `crm:E33_Linguistic_Object` instances and linked to the constraint they describe through `crm:P129_is_about`.

## 🛠️ Alignment with International Standards

| Prefix | Standard | URI |
| :--- | :--- | :--- |
| `crm` | **CIDOC CRM** | `http://www.cidoc-crm.org/cidoc-crm/` |
| `lrmoo` | **LRMoo** | `http://iflastandards.info/ns/lrm/lrmoo/` |
| `skos` | **SKOS** | `http://www.w3.org/2004/02/skos/core#` |
| `prov` | **PROV-O** | `http://www.w3.org/ns/prov#` |
| `dcterms` | **Dublin Core Terms** | `http://purl.org/dc/terms/` |
| `schema` | **Schema.org** | `http://schema.org/` |

## 📁 Repository Structure

```text
desmos/
├── data/
│   ├── ontology/
│   │   └── desmos.owl
│   └── rdf/
│       ├── concept.ttl
│       └── corpus.ttl
├── img/
│   ├── 1.png
│   ├── 2.png
│   ├── 3.png
│   ├── 4.png
│   └── 5.png
└── README.md
```

* **`data/ontology/desmos.owl`**: main DeSMòS ontology, serialized in RDF/XML.
* **`data/rdf/concept.ttl`**: RDF data for the controlled concepts and vocabularies used by the model, serialized in Turtle.
* **`data/rdf/corpus.ttl`**: RDF data for the corpus used as the DeSMòS case study, serialized in Turtle.
* **`img/`**: graphical documentation of the ontology and its main modeling components.
* **`OOPSevaluation/`**: reports produced through **OOPS! (OntOlogy Pitfall Scanner!)** and ontology validation checks.

**Author:** Enrica Bruno  
**Version:** 1.1.0  
**License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
