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
| `intro` | **INTRO** | `https://w3id.org/lso/intro/beta202506#` |

## 📖 Documentation

The HTML documentation of DeSMòS is generated using [LODE 2.0 (Live OWL Documentation Environment)](https://lode.opencitations.net/) and published through GitHub Pages.

The documentation is accessible at https://w3id.org/desmos/.

### LODE References

- Pasqual, V., Nazari, A., & Peroni, S. (2026). Supporting the understanding of ontologies for scientific knowledge graphs with the new version of LODE. In *Proceedings of the 6th International Workshop on Scientific Knowledge: Representation, Discovery, and Assessment (Sci-K 2026)*. CEUR Workshop Proceedings, 4291, 12–26. https://ceur-ws.org/Vol-4291/paper1.pdf

- Pasqual, V., Peroni, S., & Nazari, A. (2026). *LODE – Live OWL Documentation Environment* [Software]. Zenodo. https://doi.org/10.5281/zenodo.21805185


## 📁 Repository Structure

```text
desmos/
├── data/
│   ├── ontology/
│   │   └── desmos.owl
│   ├── rdf/
│   │   ├── concept.ttl
│   │   └── corpus.ttl
│   └── csv/
├── docs/
│   ├── index.html
│   ├── index.jsonld
│   ├── index.nt
│   ├── index.rdf
│   ├── index.ttl
│   ├── resources/
│   └── static/
├── evaluation/
│   ├── oops/
│   │   ├── README.md
│   │   └── oops-report.pdf
│   └── shacl/
│       └── shacl.ttl
├── img/
│   ├── 1.png
│   ├── 2.png
│   ├── 3.png
│   ├── 4.png
│   ├── 5.png
│   └── tonietto.png
├── .gitignore
└── README.md
```

* **`data/ontology/desmos.owl`**: main DeSMòS ontology, serialized in RDF/XML.
* **`data/rdf/concept.ttl`**: RDF data for the controlled concepts and vocabularies used by the model, serialized in Turtle.
* **`data/rdf/corpus.ttl`**: RDF data for the corpus used as the DeSMòS case study, serialized in Turtle.
* **`data/csv/`**: source tabular data used to populate the knowledge base; the RDF datasets in `data/rdf/` were generated from these files.
* **`docs/`**: static documentation of the DeSMòS ontology, generated using LODE 2.0 and published through GitHub Pages.
* **`evaluation/shacl/shacl.ttl`**: SHACL shapes used to validate `data/rdf/concept.ttl` and `data/rdf/corpus.ttl` against the constraints of the DeSMòS ontology.
* **`evaluation/oops/oops-report.pdf`**: report of the ontology evaluation performed with OOPS! (OntOlogy Pitfall Scanner!).
* **`evaluation/oops/README.md`**: documentation and assessment of the pitfalls identified by OOPS!.
* **`img/`**: graphical documentation of the ontology and its main modeling components.

**Author:** Enrica Bruno  
**Version:** 1.2.0  
**License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
