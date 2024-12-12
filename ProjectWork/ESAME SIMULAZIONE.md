# Documento analisi
---
- Requisiti funzionali
- Requisiti non funzionali
- Diagramma ER DB
- Wireframes (Obbligatorio per web, e opzionale anche mobile)
- Esempi dei richieste REST(Risposta, URL, )
- Budget e calcolo costi. PM 
- GANT tempi che serviranno per implementare il sistema e le figure che servono anche accenno riunioni con il cliente e stack holders
- Architettura del progetto
- Vincoli

# Contesto
---
**L’azienda Pentathlon**, catena di un **noto marchio di articoli sportivi**, richiede lo sviluppo di un sistema informativo per offrire il **servizio di noleggio degli articoli** e la **gestione del proprio magazzino**. L’applicazione deve offrire una serie di funzionalità, suddivise nelle seguenti aree:

1.	**gestione elenco materiale**: è necessario disporre di un inventario con i dati degli articoli, ad esempio: materiale di consumo e strumentazione. Per ciascun articolo si devono disporre degli attributi quali: **tipologia (a titolo di esempio sci/scarponi/racchette etc...)**, **marca, dimensioni** (**misure di scarpe, taglia degli indumenti)**, **numero di pezzi in possesso e disponibili, costo del noleggio riferito al periodo richiesto (alta o bassa stagione)**.

2.	**gestione clienti:** è necessario disporre di un archivio contenente i dati relativi ai **clienti del negozio**. Nel dettaglio, sarà necessario possedere le informazioni del cliente, poter profilare le sue richieste, **le informazioni relative alle diverse metodologie di pagamento (es. carta di credito, Paypal)** e il dettaglio della **tessera fedeltà consegnata** all’utente, al **momento della registrazione**. 
 
3.	**gestione noleggi**: è necessario disporre di un archivio contenente i **dati relativi ai noleggi**, questi comprendono: **cliente, materiale, data di inizio e fine noleggio, costo del noleggio ed eventuale sconto**.

## Il flusso logico dell’uso del sistema deve prevedere i seguenti passaggi:
---
A.	gli **impiegati** del supermercato **pubblicano e aggiornano una lista di prodotti prenotabili tramite l'applicazione**; da considerare che gli **articoli sono associati ad una categoria merceologica** per consentirne la facile selezione da parte dei clienti;
B.	**i clienti** interessati al servizio, usufruendo l'applicazione, **selezionano i prodotti desiderati e preparando la lista della spesa**. Per poter accedere al servizio, ogni cliente **deve aver effettuato l’autenticazione** (previa registrazione); Da tenere presente che i **clienti vengono identificati attraverso la carta fedeltà** in loro possesso **durante il noleggio effettuato in negozio**.
C.	**la prenotazione è ritirabile nel negozio indicato nell’applicazione**; quando **il cliente si trova in prossimità** del supermercato, tramite geo-localizzazione del dispositivo utilizzato, **l’informazione viene trasmessa ai commessi**, incaricati alla consegna;
D.	**gli addetti alle consegne sono costantemente informati sui clienti in arrivo e sul materiale da consegnare**.

L'applicazione Pentathlon deve prevedere delle opportune interfacce per permettere agli impiegati del supermercato, di gestire la lista dei prodotti da consegnare ai clienti e di di tenere monitorata la situazione. È inoltre richiesta l'implementazione di tutti gli accorgimenti necessari per garantire la privacy e il corretto trattamento dei dati personali, la sicurezza dei pagamenti, la disponibilità del servizio.
## Introduzione del progetto
---
Creazione di un software mobile (Android e iOS), e un sito web per Desktop ai fini di facilitare la gestione dei prodotti (in magazzino), degli utenti (clienti e dipendenti) e noleggi dei prodotti per la Pentathlon.
### Requisiti principali
---
- **Scalabilita'**: il progetto deve poter sostenere un numero elevato di utenti (essendo parte di una catena di un noto marchio)
- **Sicurezza**: il progetto deve essere il piu' sicuro possibile - Tutti i dati sensibili di utenti e prodotti devono essere protetti e gestiti secondo i regolamenti del GDPR (General Data Protection Regulation).
- **Usabilita'**: il progetto deve essere facile da utilizzare, intuitivo, efficiente e veloce.

**Stakeholders coinvolti**:
- Utenti: desiderano un'esperienza piu' piacevole e veloce.
- Impiegati: hanno bisogno una procedura di gestione di dati, prodotti e clienti piu' semplice, intuitiva e veloce. 
- Manager: ha bisogno di un sistema per la gestione degli impiegati e la visione dei prodotti presenti piu' efficiente e intuitiva.
- Team di marketing: hanno bisogno di un sistema per vedere piu' velocemente quali prodotti sono i piu' noleggiati, quali meno e quali proprio non vengono noleggiati. 
### Requisiti funzionali
---
