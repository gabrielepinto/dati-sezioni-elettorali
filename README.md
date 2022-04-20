![immagine](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/immagine_copertina.PNG)
# dati e shapefile delle sezioni elettorali italiane
Questo repository contiene gli shapefile delle sezioni elettorali italiane insieme ad una raccolta dei risultati elettorali a livello di sezione per alcune città italiane (al momento Roma, Milano e Torino). Il repository è un "work-in-progress" e verrà costantemente aggiornato con altre città/elezioni nel prossimo futuro.

I dati pubblicati in questo repository sono il risultato di un progetto di ricerca la cui metodologia è descritta in questo paper:

La diffusione e utilizzo di dei dati contenuti in questo repository per scopi di ricerca e no-profit è permessa a titolo gratuito a conto che la fonte e l'autore siano espressamente citati. Per citare i dati utilizzare la seguente citazione:

L'utilizzo dei dati contenuti nel repository per scopi commerciali o similia non è autorizzata senza previa autorizzazione scritta dell'autore.


## shapefile
Gli shapefile che geolocalizzano le aree in cui sono localizzate le sezioni elettorali possono essere trovate sotto la cartella ![shapefiles sezioni elettorali](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali).
Per ogni comune, sono presenti due tipi di file: "precincts_voronoi" e "precincts_census". La differenza tra i due file è da ricondurre alle due diverse procedure utilizzate per ricostruire i poligoni nelle sezioni (a partire dai viari elettorali ufficiali forniti dai comuni). Entrambe le procedure sono descritte estensivamente in questo paper.

## risultati elettorali
I risultati elettorali coprono un periodo che va (circa) dal 2001 al 2021 (in costante aggiornamento) per varie tipologie di elezioni a seconda della disponibilità dei dati ufficiali che variano da comune a comune. L'archivio include i risultati a livello di sezione per referendum, voti di preferenza, elezioni sub-comunali (municipi, circoscrizioni, etc...), comunali, politiche, regionali, europee... tutti i file possono essere scaricati dall'archivio in formato rar che trovate ![qui](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/risultati_elettorali.rar): 
Per la lista della descrizione dei singoli file dei risultati elettorali consultare il file ![anagrafica completa](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/anagrafica_completa_all_cities.csv)

I dati contenuti nell'archivio sono il frutto di un lavoro di pulizia dei file originali disponibili nelle sezioni "open-data" dei vari comuni e possono essere facilmente "fusi" (merged) con gli shapefile utilizzando la chiave "SEZIONE" contenuta in tutti i file.

## dati censimento per sezione
La cartella  ![censimento sezioni elettorali](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/dati_censimento_sezione_elettorale) riporta per ogni citta il valore delle variabili censuarie ISTAT (2011) per ogni sezione elettorale calcolate con interpolazione spaziale . Oltre alle variabili standard fornite da ISTAT sono presenti anche una serie di indicatori (tasso di istruzione, cittadinanza etc...). La descrizione delle variabili è riportata nel file "tracciato_variabili.csv".

## F.A.Q.

_A quale versione del viario elettorale corrispondono le sezioni elettorali?_ 
L'ultima disponibile. Generalmente, Settembre 2021.


