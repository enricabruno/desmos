# Report di Validazione DeSMòS

In questo file è archiviata la documentazione relativa alla qualità dell'ontologia DeSMòS, generata tramite il tool **OOPS! (OntOlogy Pitfall Scanner!)**.

## Evoluzione e Miglioramento (Versione Preliminare vs Versione 1)
Questa validazione si riferisce alla **Versione 1.1.0** del modello. Rispetto alla versione preliminare (**Version 1.0.0**), il processo di rifinitura ha permesso di eliminare diverse criticità minori, consolidando la struttura logica e l'interoperabilità del namespace `desmos:`.

Il processo di revisione iterativa ha portato a un drastico abbattimento delle criticità rilevate inizialmente:
* Risoluzione del Pitfall P08 (Missing Annotations): Nella versione v1.0.0 erano stati rilevati 16 casi di annotazioni mancanti per elementi fondamentali come F1 Work, F2 Expression e E39 Actor. Nella versione v1.1.0, questo pitfall è stato completamente eliminato.
* Risoluzione del Pitfall P13 (Inverse relationships): La versione v1.0.0 presentava 8 casi di relazioni inverse non dichiarate esplicitamente. Nella versione v1.1.0, tutte le relazioni inverse necessarie sono state implementate, risolvendo integralmente la segnalazione.
* Consolidamento Strutturale: Il modello v1.1.0 mantiene solo le segnalazioni legate alla necessaria interoperabilità con standard esterni, confermando la maturità del namespace `desmos:`.

## Sintesi dei Risultati (Versione 1)
L'analisi automatizzata ha assegnato al modello il badge **"Minor Pitfalls"**. Questo indica l'assenza di errori critici o importanti che possano influenzare la coerenza logica o l'applicabilità dell'ontologia .
* **Pitfall Rilevati**: 2 casi di livello "Minor".
* **Stato del Namespace**: 0 pitfall rilevati per le entità originali introdotte dal modello.
* **Suggerimenti**: 2 segnalazioni riguardanti la possibile definizione di proprietà simmetriche o transitive

## Giustificazione dei Pitfall Residui
Le segnalazioni di livello "Minor" rilevate nel report v1.1.0 sono state mantenute intenzionalmente per preservare l'allineamento con gli standard internazionali dei beni culturali (CIDOC CRM e LRMoo):

* **P07 (Merging different concepts in the same class)**: Rilevato per la classe http://www.cidoc-crm.org/cidoc-crm/E29 Design or Procedure. Si tratta di un **falso positivo** dovuto alla nomenclatura dello standard CIDOC CRM: la congiunzione "or" è parte del nome ufficiale della classe e non indica una fusione impropria di concetti differenti.
* **P22 (Using different naming conventions in the ontology)**: Segnalato come pitfall generale di livello "Minor" . La discrepanza deriva dalla coesistenza tra la convenzione CamelCase adottata per DeSMOS e la nomenclatura alfanumerica dello standard CIDOC CRM (es. E29_Design_or_Procedure), fondamentale per garantire l'interoperabilità del sistema.

---
*Validazione eseguita in data 15/04/2026.*