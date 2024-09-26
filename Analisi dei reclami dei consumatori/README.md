# Analisi dei reclami dei consumatori

### Dataset

[Link al dataset](https://github.com/Profession-AI/progetti-excel/raw/main/Analisi%20dei%20reclami%20dei%20consumatori/customers_complaints_assignment.xlsx)

### Obiettivo del Progetto
Il progetto è commissionato da **FinServ Solutions**, una compagnia specializzata in soluzioni software per la gestione dei reclami dei clienti nel settore finanziario. L’obiettivo è migliorare l’efficacia nell’analisi dei reclami dei clienti tramite la ristrutturazione e la personalizzazione di un foglio di calcolo, al fine di ottimizzare l'accesso alle informazioni e il processo decisionale.

### Motivazione
L’azienda ha notato che l’attuale struttura del foglio di calcolo utilizzato per la gestione dei reclami presenta inefficienze, rendendo difficoltosa la lettura dei dati, l'estrazione di insight e l’analisi geografica. Una revisione mirata del foglio di calcolo migliorerà la visibilità dei dati critici, consentendo una più rapida identificazione dei problemi e ottimizzando la risposta aziendale ai clienti. Inoltre, una riorganizzazione grafica e funzionale permetterà al team di servizio clienti di operare con maggiore agilità.

### Valore Aggiunto Atteso
- **Miglioramento dell’analisi geografica**: La creazione di un tab dedicato agli insights geografici faciliterà l’identificazione delle aree con il maggior numero di reclami, consentendo azioni mirate.
- **Maggiore efficienza nel processo decisionale**: Grazie all’aggiunta di un tab statistico e alla possibilità di filtrare i dati, il team potrà individuare rapidamente le problematiche più frequenti, permettendo una risposta più rapida e adeguata.
- **Ottimizzazione del tempo di risposta**: La nuova struttura evidenzierà automaticamente i tempi di risoluzione dei reclami, offrendo un monitoraggio più efficace delle performance aziendali.
## Cosa devi fare

Per realizzare il progetto, dovrai modificare il foglio di calcolo allegato in modo da fargli avere la seguente struttura:

### Primo tab o scheda
**Nome**: "Consumer complaints"

**Stile**:
- La prima riga di intestazione ha carattere Comics Sans MS, dimensione 12pt e colore blu, riquadrata su 4 lati con bordo doppio.
- Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile.
- Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco senza bordi righe e colonne a contorno dei veri e propri dati).
- Le date presenti (colonne `Date received` e `Date sent to company`) hanno la data in formato dd/mm/yy.

**Contenuto**:
- Una colonna in fondo che contiene il numero di giorni effettivi intercorsi fra la data di invio e quella di ricezione della comunicazione.
- Il foglio di calcolo contiene righe ordinate in modo crescente sul valore della colonna `Complaint ID`.
- È presente un filtro sulla colonna `Date received`, che permette la visualizzazione delle sole righe con data antecedente al 8 agosto 2016.

### Secondo tab o scheda
**Nome**: "Geographical insights"

**Stile**:
- La prima riga di intestazione ha carattere Comics Sans MS, dimensione 12pt e colore blu, riquadrata su 4 lati con bordo doppio.
- Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile.
- Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco senza bordi righe e colonne a contorno dei veri e propri dati).
- La riga di intestazione contiene i seguenti titoli:
    - Number of complaints per state
    - Percentage of complaints per state
- È presente una colonna di intestazione che contiene tutte le sigle degli stati presenti nel tab "Consumer complaints"

**Contenuto**:
- Nella colonna B è riportato il numero di lamentele presenti nel tab principale suddivise per stato. *(Hint: utilizzare la funzione `CONTA.SE`)*.
- Nella colonna C è riportato il numero percentuale (arrotondato all'intero successivo) di lamentele presenti nel tab principale suddivise per stato. La cella è di colore verde se tale percentuale è inferiore al 2%, rossa altrimenti. *(Hint: formattazione condizionale)*.

### Terzo tab o scheda
**Nome**: "Statistical insights"

**Stile**:
- La prima riga di intestazione ha carattere Comics Sans MS, dimensione 12pt e colore blu, riquadrata su 4 lati con bordo doppio.
- Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile.
- Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco senza bordi righe e colonne a contorno dei veri e propri dati).
- La riga di intestazione contiene i seguenti titoli:
    - Distinct issues

**Contenuto**:
- Nella colonna A sono riportati tutti i possibili motivi di reclamo (valori distinti della colonna `Issues` del tab principale).
- Nella cella B7 si riporta il valore moda (il più frequente) fra tutte le categorie di reclami. *(Hint: contare le occorrenze delle varie issue e fare la moda fra i valori numerici)*.

# Modalità di consegna: file Excel creato