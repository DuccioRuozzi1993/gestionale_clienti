# CRM Bancario

**CRM single-page per la gestione clienti in ambito bancario e finanziario.**  
Un'applicazione web completa, contenuta in un unico file HTML, progettata per gestori e consulenti che vogliono organizzare relazioni commerciali, trattative, campagne e budget di vendita — tutto offline e senza dipendenze server.

![Version](https://img.shields.io/badge/versione-1.0-blue)
![License](https://img.shields.io/badge/licenza-MIT-green)

---

## Caratteristiche principali

### 📋 Lista del giorno
Sistema intelligente di prioritizzazione giornaliera dei clienti da contattare. L'algoritmo considera scadenze, follow-up in ritardo, frequenza di contatto e campagne attive, generando batch giornalieri con un meccanismo di cooldown per evitare duplicazioni.

### 👥 Gestione clienti
Anagrafica completa con codice CDG, ragione sociale, settore, rating e categorizzazione (privato/azienda). Ogni scheda cliente include tab dedicati per anagrafica, referenti, bisogni, contatti, impegni futuri, trattative e vendite.

### 🔥 Pipeline trattative
Gestione delle trattative commerciali con fasi progressive: Interesse → Proposta → In delibera → Chiusa (vinta/persa). Visualizzazione con indicatori di valore e scadenze follow-up.

### 📢 Campagne
Organizzazione di campagne commerciali con liste clienti target. Supporta campagne pinned che alimentano automaticamente la lista del giorno.

### 💰 Budget & Avanzamento
Definizione di obiettivi di vendita per prodotto (in euro o pezzi), registrazione vendite e monitoraggio dell'avanzamento rispetto ai target con grafici Chart.js.

### ⚙️ Impostazioni
Gestione tag personalizzati per bisogni, settori e tipologie di contatto. Configurazione prodotti budget, dimensione batch giornaliero e monitoraggio dello spazio localStorage utilizzato.

### 🗑 Cestino
Soft-delete con possibilità di ripristino per clienti, referenti, contatti, impegni, trattative e vendite.

### 🔍 Ricerca globale
Ricerca istantanea su tutti i clienti per CDG, ragione sociale o referente.

### 💾 Backup & Ripristino
Esportazione e importazione dello stato completo in formato JSON. I dati sono persistiti in `localStorage`.

---

## Requisiti

Nessuno. Basta un browser moderno:

- Google Chrome (consigliato)
- Firefox
- Safari
- Edge

Non richiede server, database, installazione o connessione internet (dopo il primo caricamento dei font Google).

---

## Utilizzo

1. Scarica il file `crm_fase3.html`
2. Aprilo nel browser
3. Inizia ad aggiungere clienti

I dati vengono salvati automaticamente nel `localStorage` del browser.

> **⚠️ Nota:** i dati sono legati al browser e al dispositivo. Usa la funzione di backup (JSON) per trasferirli o per sicurezza.

---

## Stack tecnico

| Componente | Tecnologia |
|---|---|
| Frontend | HTML5, CSS3, JavaScript vanilla |
| UI fonts | Cormorant Garamond, Jost (Google Fonts) |
| Grafici | Chart.js 4.4.1 (CDN) |
| Persistenza | localStorage |
| Architettura | Single-file, zero dipendenze server |

---

## Struttura dati

Lo stato dell'applicazione è un oggetto JSON salvato in `localStorage` con chiave `crmBancario`. Contiene:

- `clienti` — array di oggetti cliente con referenti, contatti, impegni e bisogni annidati
- `trattative` — array di trattative commerciali collegate ai clienti
- `budget` — obiettivi e vendite per prodotto
- `campagne` — campagne commerciali con liste target
- `cestino` — elementi eliminati recuperabili
- `impostazioni` — tag personalizzati, prodotti e configurazione

---

## Licenza

Questo progetto è rilasciato sotto licenza [MIT](LICENSE).

---

## Autore

**Duccio Ruozzi** — Marzo 2026
