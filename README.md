![immagine](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/immagine_copertina.PNG)
# dati e shapefile delle sezioni elettorali italiane
Questo repository contiene gli shapefile delle sezioni elettorali italiane insieme ad una raccolta dei risultati elettorali a livello di sezione per alcune città italiane (al momento Roma, Milano e Torino). Il repository è un "work-in-progress" e verrà costantemente aggiornato con altre città/elezioni nel prossimo futuro.

I dati pubblicati in questo repository sono il risultato di un progetto di ricerca la cui metodologia è descritta in ![questo paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4096926):

La diffusione e utilizzo di dei dati contenuti in questo repository per scopi di ricerca e no-profit è permessa a titolo gratuito a conto che la fonte e l'autore siano espressamente citati. Per citare i dati utilizzare la seguente citazione: 
 -Pinto, Gabriele, Building geolocated precinct boundaries from voter's address lists: the Italian case (April 29, 2022). Available at SSRN: https://ssrn.com/abstract=4096926

L'utilizzo dei dati contenuti nel repository per scopi commerciali o similia non è autorizzata senza previa autorizzazione scritta dell'autore.

## anteprima dati
un app  per visualizzare in anteprima una parte dei dati è disponibile qui:https://sezionielettorali.herokuapp.com/

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

1. _Come posso aprire gli shapefile delle sezioni elettorali?_
Dopo aver scaricato gli shapefile dalla ![cartella](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali) questi possono essere aperti e visualizzati utilizznado qualsiasi software GIS open-source o a pagamento (es: ![QGIS](https://qgis.org/en/site/forusers/download.html)).
In alternativa, gli shapefile possono essere letti "online" effettuando una richiesta direttamente al repository. Per un esempio con Python vedere ![questo notebook]!(https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/esempio_apertura_file.ipynb).

2. _A quale versione del viario elettorale corrispondono le sezioni elettorali?_  
L'ultima disponibile. Generalmente, Settembre 2021. 

3. _Qual'è la fonte dei risultati elettorali ?_ 
La fonte sono le sezioni open-data dei comuni italiani. Poichè i comuni forniscono in dati in formati non inter-operabili questi sono stati "puliti" tramite varie procedure e ricondotti in unici file per ogni elezione. Ad esempio, l'archivio online del  ![comune di roma](https://www.elezioni.comune.roma.it/archivio.asp) con i risultati elettorali a livello di sezione è composta da oltre 5000 file excel (un file per ogni lista, etc...) che seguono (spesso) formattazioni diverse. Questi sono stati ricondotti ad un unico file per ogni elezione utilizzando per aumentarne la fruibilità. Ragionamenti simili valgono per i comuni di ![Torino](http://aperto.comune.torino.it/dataset?dcat_subtheme_it=0416+procedura+elettorale+e+voto) e ![Milano](https://dati.comune.milano.it/dataset?tags=elezione)



