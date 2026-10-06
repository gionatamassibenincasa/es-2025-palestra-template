# `ASSIGNMENTS.md`

```markdown
# Progetto Didattico: Gestione Informatizzata Palestra (Esame di Stato M733 - 2005)

```

---

## 📌 Panoramica del Progetto

Il presente progetto richiede la progettazione e la prototipazione del sistema informativo per una **palestra** che intende informatizzare la gestione dei corsi, degli istruttori, delle iscrizioni, del monitoraggio delle presenze e della situazione contabile dei clienti.

Il progetto include anche un approfondimento teorico sulle tematiche del **telelavoro** e dell'**e-commerce** nei contesti organizzativi moderni.

---

## 🎯 Obiettivi Didattici

Al termine dell'attività, lo studente sarà in grado di:

1. **Analizzare un testo d'esame** estraendo requisiti, entità, attributi e relazioni.
2. **Elaborare un Glossario di dominio** formale e strutturato.
3. **Modellare la base di dati** mediante diagrammi PlantUML (modello concettuale ed E-R ristrutturato per modello relazionale).
4. **Implementare lo schema relazionale in SQLite** applicando i vincoli d'integrità referenziale e i domini dei dati.
5. **Popolare il database** con dati di test realistici per effettuare la verifica funzionale.
6. **Formulare query SQL** per rispondere ai requisiti informativi aziendali.
7. **Sviluppare un prototipo di applicazione web in PHP** per l'interazione degli utenti con il database SQLite.
8. **Redigere una relazione sintetica** sugli aspetti socio-economici e tecnologici legati a telelavoro ed e-commerce.

---

## 📂 Struttura della Repository Richiesta

Per completare l'assegnazione su Classroom 50, la repository di progetto deve rispettare rigorosamente l'alberatura seguente:

```text
.
├── ASSIGNMENTS.md
├── testo_analizzato.md
├── glossario.md
├── modello_concettuale.plantuml
├── modello_logico.plantuml
├── schema.sql
├── popolamento.sql
├── query.sql
├── web_app/
│   ├── db.php
│   └── iscrizione.php
└── quesiti/
    └── quesito_1.md

```

---

## 📋 Lista dei Consegnabili (Task Checklist)

### Task 1: Analisi del Testo (`testo_analizzato.md`)

* [ ] Trascrivere il testo della traccia.
* [ ] Evidenziare con la convenzione concordata:
* **Grassetto**: Entità / Nomi.
* *Corsivo*: Attributi.
* <u>Sottolineato</u>: Associazioni / Verbi.



### Task 2: Glossario dei Termini (`glossario.md`)

* [ ] Compilare la tabella Markdown contenente:
* Termine.
* Sinonimi / Omonimi.
* Descrizione di dominio.
* Termini correlati.



### Task 3: Modellazione Concettuale (`modello_concettuale.plantuml`)

* [ ] Disegnare le classi di analisi con PlantUML.
* [ ] Definire tutte le entità individuate nell'analisi.
* [ ] Inserire i relativi attributi.
* [ ] Indicare le associazioni e le cardinalità (1:1, 1:N, N:M).

### Task 4: Modellazione Logica (`modello_logico.plantuml`)

* [ ] Ristrutturare il modello per il sistema relazionale.
* [ ] Esplicitare Chiavi Primarie (`<>`) e Chiavi Esterne (`<>`).
* [ ] Trasformare le relazioni N:M in tabelle di associazione.

### Task 5: DDL Database SQLite (`schema.sql`)

* [ ] Abilitare i vincoli sulle chiavi esterne (`PRAGMA foreign_keys = ON;`).
* [ ] Scrivere le istruzioni `CREATE TABLE` con tipi di dato corretti.
* [ ] Dichiarare le chiavi primarie, le chiavi esterne e i vincoli `NOT NULL`, `UNIQUE`, `CHECK`.

### Task 6: Popolamento Database (`popolamento.sql`)

* [ ] Inserire dati di test tramite istruzioni `INSERT INTO`.
* [ ] Garantire la presenza di record per tutte le tabelle (almeno 3-5 record per tabella).

### Task 7: Interrogazioni SQL (`query.sql`)

* [ ] Rispondere ai quesiti posti dalla traccia d'esame.
* [ ] Scrivere query corrette, leggibili e ottimizzate con clausole `JOIN`, `GROUP BY`, `WHERE`.

### Task 8: Prototipo Web PHP (`web_app/`)

* [ ] Implementare la connessione PDO a SQLite in `db.php`.
* [ ] Creare il form HTML/PHP per l'iscrizione ai corsi o consultazione in `iscrizione.php`.
* [ ] Effettuare la validazione dei dati in input e la gestione degli errori.

### Task 9: Relazione Teorica (`quesiti/quesito_1.md`)

* [ ] Trattare il punto 1 della traccia in formato Markdown.
* [ ] Analizzare gli aspetti tecnologici, organizzativi e socio-economici di telelavoro ed e-commerce.

---

## 📊 Rubrica di Valutazione (Classroom 50)

| Criterio | Punti Max | Descrittori di Valutazione |
| --- | --- | --- |
| **Analisi e Glossario** | 10 | Completezza dell'individuazione di entità/attributi/associazioni e precisione del glossario. |
| **Modellazione Concettuale e Logica** | 25 | Correttezza dei diagrammi PlantUML, rispetto delle regole di normalizzazione e corretta definizione delle FK/PK. |
| **Database SQL (DDL, DML, Query)** | 25 | Sintassi SQLite valida, vincoli rispettati, popolamento coerente ed esecuzione corretta delle query richieste. |
| **Sviluppo Web (PHP + SQLite)** | 25 | Funzionalità del form, integrazione PDO con il database, gestione dell'input ed usabilità dell'interfaccia. |
| **Relazione Teorica** | 15 | Proprietà di linguaggio, approfondimento dei temi tecnologici, organizzativi e socio-economici. |
| **TOTALE** | **100** |  |

---

## ⏰ Modalità e Tempi di Consegna

* **Tempo a disposizione:** 6 ore (simulazione d'esame) oppure consegna entro la data stabilita su Classroom 50.
* **Invio:** Effettuare il `commit` ed il `push` di tutti i file nella repository del progetto su Classroom 50 prima dello scadere del termine.
