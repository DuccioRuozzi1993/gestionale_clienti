# 🏦 Task Manager Light

Un task manager pensato per chi lavora nel caos — filiali bancarie, uffici, reception, chiunque venga sommerso da interruzioni continue e deve decidere al volo cosa fare, cosa parcheggiare e cosa non dimenticare.

Non è un to-do generico. È un sistema di triage.

## Il problema che risolve

Lavori in un ambiente dove tutto sembra urgente: il telefono squilla, arriva una mail dalla direzione, un cliente chiede qualcosa allo sportello, un collega ti ferma al volo. Nel caos segui solo le cose percepite come urgenti e lasci indietro quelle importanti — finché è troppo tardi.

Task Manager Light ti protegge da questo pattern con quattro colonne, zero navigazione e meccanismi visivi che rendono impossibile dimenticare.

## Come funziona

**Una schermata, quattro colonne:**

- **Inbox** — ci butti tutto in 5 secondi, senza pensare
- **Oggi** — le 3-5 cose che hai scelto per la giornata
- **In attesa** — pratiche parcheggiate, con nome di chi ti deve rispondere e contatore dei giorni
- **Backlog** — tutto il resto, con evidenza visiva sulle cose che invecchiano

**Il flusso quotidiano:**

1. Arriva qualcosa → scrivi nella barra, Invio, finisce in Inbox
2. Hai 2 minuti di buco → smisti: trascini le cose dove servono
3. Fine giornata → completi, il giorno dopo riparti

## Funzionalità

- **Input rapidissimo** — scrivi e premi Invio (Inbox) o Ctrl+Invio (diretto in Oggi)
- **Drag & drop** — tra colonne e dentro le colonne per riordinare
- **Invecchiamento visivo** — le task nel backlog diventano arancioni dopo 3 giorni, rosse dopo 7
- **Scadenze** — con evidenza progressiva: fra 3g → domani → oggi → scaduta (con pulsazione)
- **In attesa di...** — ogni pratica parcheggiata mostra chi la blocca e da quanti giorni
- **Checklist** — passaggi spuntabili dentro ogni task, con progresso visibile sulla card (es. 3/5)
- **Note** — campo libero per dettagli, numeri pratica, riferimenti
- **Task ricorrenti** — giornaliere, settimanali, mensili. Si ricreano automaticamente al completamento
- **Banner "task da ieri"** — se hai lasciato cose in "Oggi" dal giorno prima, te lo dice
- **Limite morbido** — se metti più di 5 task in "Oggi", il contatore diventa rosso
- **Ricerca** — Ctrl+K, cerca nel testo, nelle note e nei nomi di attesa
- **Categorie** — Amm/Compliance, Clienti, Uffici/Direzione, Interno (con filtri)
- **Contatore nel tab** — "🎯 3 | Filiale" visibile anche senza cliccare sul tab
- **Annulla cancellazione** — toast con countdown di 5 secondi per recuperare task eliminate
- **Backup** — esporta/importa JSON per sicurezza
- **Animazione di completamento** — micro-soddisfazione a ogni task chiusa

## Requisiti

Nessuno. È un singolo file HTML. Serve solo un browser.

## Installazione

1. Scarica `filiale-task-manager.html`
2. Doppio click → si apre nel browser
3. Opzionale: aggiungilo ai preferiti (Ctrl+D)

## Dati e privacy

Tutti i dati restano nel browser (localStorage). Nessun server, nessun account, nessun tracciamento. I dati vivono sul tuo PC e non escono mai.

Fai backup regolari con il bottone 💾 se usi lo strumento per lavoro.

## Scorciatoie da tastiera

| Scorciatoia | Azione |
|---|---|
| `Invio` | Aggiungi task in Inbox |
| `Ctrl+Invio` | Aggiungi task in Oggi |
| `Ctrl+K` | Apri/chiudi ricerca |
| `Esc` | Chiudi modale/ricerca |
| `Doppio click` | Modifica testo task |

## Per chi è

- Operatori di filiale bancaria
- Chiunque lavori con interruzioni continue
- Chi ha bisogno di uno strumento veloce senza setup
- Chi non vuole registrarsi a nulla

## Per chi non è

- Team che hanno bisogno di collaborazione in tempo reale
- Chi cerca integrazioni con email/calendar
- Chi ha bisogno di sync tra dispositivi

## Stack

- HTML + CSS + React 18 (via CDN)
- localStorage per la persistenza
- Zero dipendenze da installare
- Zero build step

## Autore

**Duccio Ruozzi** — nato dall'esigenza di gestire task che si accumulano in contesti caotici.

## Licenza

MIT — vedi [LICENSE](LICENSE) per i dettagli.
