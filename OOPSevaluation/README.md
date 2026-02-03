# Report di Validazione DeSMòS

In questa cartella è archiviata la documentazione relativa alla qualità dell'ontologia, generata tramite il tool **OOPS! (OntOlogy Pitfall Scanner!)**.

## Sintesi dei Risultati
* **Namespace `desmos:`**: 0 pitfall rilevati.
* **Pitfall Minor Residui**: 16 casi di annotazioni mancanti e 8 di relazioni inverse non dichiarate.

## Giustificazione dei Pitfall Residui
I risultati mostrati nel file `oops_report.html` indicano alcuni pitfall di livello "Minor" che sono stati mantenuti intenzionalmente per le seguenti ragioni:

1. **P08 (Missing Annotations)**: Le mancanze riguardano esclusivamente classi e proprietà di ontologie esterne (CIDOC CRM, LRMoo, PROV-O) importate per riferimento. Non sono state aggiunte annotazioni locali per evitare ridondanze e conflitti con i namespace ufficiali.
2. **P13 (Inverse Relationships)**: Le relazioni inverse per le proprietà esterne non sono state dichiarate localmente per preservare la conformità agli standard originali.
3. **P22 (Naming Conventions)**: La coerenza stilistica è garantita all'interno del namespace `desmos:`. Le discrepanze rilevate dal tool sono dovute alla nomenclatura originale dei termini CIDOC CRM (es. uso di underscore e numeri).

---
*Validazione eseguita in data 27/01/2026.*