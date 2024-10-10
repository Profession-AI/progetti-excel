# Analisi di operazioni di trading

**FinTrack Solutions** è un'azienda innovativa che fornisce strumenti avanzati per il monitoraggio e l'analisi delle performance finanziarie. Questo progetto mira a migliorare e ottimizzare un foglio di calcolo esistente, che traccia le operazioni finanziarie svolte dal nostro cliente principale, **Bob**, dal 1° gennaio 2021. Il progetto offrirà un'analisi completa delle operazioni di trading e consentirà di prendere decisioni strategiche basate su dati affidabili e accuratamente strutturati.

## Obiettivo del Progetto

L'obiettivo è trasformare un semplice foglio di calcolo in uno **strumento di analisi dinamico e visivamente efficace**. Questo permetterà di ottenere insights rilevanti sulle revenue generate dal trading di azioni in diversi mercati finanziari e facilitare decisioni informate.

### Valore aggiunto per FinTrack Solutions:
- Miglioramento della gestione e analisi delle operazioni di trading.
- Implementazione di strumenti di visualizzazione interattivi che migliorano la comprensione dei dati.
- Automazione delle funzioni di analisi finanziaria, riducendo tempi e risorse necessari per l'analisi manuale.

## Dataset Fornito

Il dataset (scaricabile da qui: [https://proai-datasets.s3.eu-west-3.amazonaws.com/trades_on_exchanges.xlsx](https://proai-datasets.s3.eu-west-3.amazonaws.com/trades_on_exchanges.xlsx)) rappresenta le transazioni finanziarie registrate nel trading di azioni effettuate da Bob. Le colonne presenti nel foglio sono:

- **TradeID**: identificativo unico del trade (8 cifre).
- **Stock Exchange**: mercato in cui è stata eseguita l'operazione.
- **Region**: area geografica del mercato.
- **Date Added**: data di acquisto dell'azione (formato YYYY-MM-DD).
- **Quantity**: quantità di azioni acquistate/vendute.
- **Buy Price**: prezzo di acquisto per singola azione.
- **Date Sold**: data di vendita dell'azione (formato YYYY-MM-DD).
- **Sell Price**: prezzo di vendita per singola azione.

## Attività Richieste

### 1. **Modifica del Foglio di Calcolo**

Il foglio di calcolo verrà riorganizzato per una migliore leggibilità e una maggiore utilità operativa. Verranno create quattro schede principali, ciascuna con uno stile e una struttura specifica.

---

### **Scheda 1: "My Trades"**

Questa scheda presenta un riepilogo delle operazioni di trading effettuate.

**Stile**:
- Intestazione: carattere **Comic Sans MS** (12pt, colore blu) con bordo doppio.
- Tutte le celle non di intestazione saranno riquadrate con un bordo nero sottile.
- Le colonne "Date Added" e "Date Sold" avranno il formato data **DD/MM/YY**.

**Valore Aggiunto**: Permette di visualizzare chiaramente tutte le transazioni effettuate con formattazione coerente e personalizzata, facilitando l'analisi rapida delle operazioni.

---

### **Scheda 2: "Stock Exchanges"**

In questa scheda, si effettuerà una pivot table che raggruppa i mercati finanziari in base alla regione e riporta il numero di azioni scambiate.

**Stile**:
- Intestazione: **Comic Sans MS** (12pt, colore blu) con bordo doppio.
- Ogni cella riquadrata in nero.
  
**Contenuto**:
- **Pivot table** per visualizzare il numero di azioni scambiate per stato.
- Colonna aggiuntiva che indica se è necessario pagare tasse basate su un valore soglia di 67 azioni scambiate.

**Valore Aggiunto**: Automatizza il calcolo della tassazione e offre un quadro chiaro delle operazioni effettuate per ciascun mercato.

---

### **Scheda 3: "Profit Insights"**

Questa scheda è dedicata all'analisi del profitto ottenuto dalle operazioni di trading.

**Stile**:
- Intestazione: **Comic Sans MS** (12pt, colore blu) con bordo doppio.

**Contenuto**:
- **Colonna A**: riferimento ai TradeID della scheda "My Trades".
- **Colonna B**: durata del possesso delle azioni (calcolata in giorni).
- **Colonna C**: profitto generato da ciascun trade (differenza tra prezzo di vendita e di acquisto moltiplicata per la quantità di azioni scambiate). Formato valuta: dollaro americano con 5 cifre decimali.
- Istogramma per visualizzare la distribuzione della durata dei trade.
- **Commento** sotto il grafico per spiegare se la durata segue una distribuzione normale o meno.

**Valore Aggiunto**: Fornisce un'analisi immediata e dettagliata dei profitti, evidenziando le performance delle operazioni in relazione alla loro durata.

---

### **Scheda 4: "Number of Trades Exchanged"**

Questa scheda presenta una **tabella di contingenza** per analizzare la distribuzione del numero di trade per regione.

**Stile**:
- Intestazione: **Comic Sans MS** (12pt, colore blu).
  
**Contenuto**:
- **Tabella di contingenza** che mostra la frequenza dei trade per regione.
- Calcolo delle probabilità associate a eventi specifici di seguito riportati

Gli eventi da considerare per il calcolo delle probabilità sono:

- Probabilità che avvenga un trade nel Regno Unito con quantità uguale a 1
- Probabilità che avvenga un trade in un paese asiatico con quantità <= 8


**Valore Aggiunto**: Fornisce un'analisi probabilistica delle operazioni, aiutando a prendere decisioni strategiche basate sulle distribuzioni di trading per regione.

---

## Conclusione

Questo progetto non si limita a una semplice modifica di un foglio di calcolo, ma trasforma i dati finanziari in un potente strumento decisionale per **FinTrack Solutions**. Grazie a una struttura di facile lettura e a funzioni avanzate come tabelle pivot, analisi del profitto e distribuzioni probabilistiche, il cliente potrà monitorare le sue performance finanziarie e ottimizzare le sue operazioni di trading in modo efficace e strategico.

# Modalità di consegna: file Excel creato