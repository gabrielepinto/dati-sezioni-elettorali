![immagine](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/immagine_copertina.PNG)
# Where I can download the data?
To download electoral data at the precinct level click [here](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/risultati_elettorali.rar).   
Description of each file contained in the zipped archive can be found [here](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/anagrafica_completa_all_cities.csv).  
Precincts shapefile can be found [here](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali).  
In case you need GeoJSON check  [here](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali_geojson)

Please remember to cite the source:
<<<<<<< HEAD
 _Gabriele Pinto(2023) Sezioni Elettorali Italiane (SEI): a new database of Italian electoral results geocoded at precinct level,Political Research Exchange,5:1,DOI: 10.1080/2474736X.2023.2185158_ [https://www.tandfonline.com/doi/full/10.1080/2474736X.2023.2185158]
=======
 _Gabriele Pinto (2023) Sezioni Elettorali Italiane (SEI): a new database of Italian electoral results geocoded at precinct level, Political Research Exchange, 5:1, DOI: 10.1080/2474736X.2023.2185158_
>>>>>>> 10fe85e360987021a26fc3f158f579fb2c5d5361

# dati e shapefile delle sezioni elettorali italiane (SEI)
Questo repository contiene gli shapefile delle sezioni elettorali italiane (SEI) insieme ad una raccolta dei risultati elettorali a livello di sezione per alcune città italiane (al momento Roma, Milano, Torino, Genova, Firenze, Bologna e Palermo). Il repository è un "work-in-progress" e verrà costantemente aggiornato con altre città/elezioni nel prossimo futuro.

I dati pubblicati in questo repository sono il risultato di un progetto di ricerca la cui metodologia è descritta in [questo paper](https://www.tandfonline.com/doi/full/10.1080/2474736X.2023.2185158):

La diffusione e utilizzo di dei dati contenuti in questo repository per scopi di ricerca e no-profit è permessa a titolo gratuito a conto che la fonte e l'autore siano espressamente citati. Per citare i dati utilizzare la seguente citazione: 

 _Gabriele Pinto(2023) Sezioni Elettorali Italiane (SEI): a new database of Italian electoral results geocoded at precinct level,Political Research Exchange,5:1,DOI: 10.1080/2474736X.2023.2185158_ [https://www.tandfonline.com/doi/full/10.1080/2474736X.2023.2185158]

L'utilizzo dei dati contenuti nel repository per scopi commerciali o similia non è autorizzata senza previa autorizzazione scritta dell'autore.


## aggiornamenti/updates
ultimo aggiornamento: elezioni regionali 2023. Sono stati aggiunti i risultati per sezioni delle elezioni regionali 2023 nel Lazio e in Lombardia. 
!!! in data 16/12/2022 sono stati aggiornati i file dei dati di censimento che contenevano un errore. Inoltre sono stati aggiunti i dati per i censimenti del 1991 e 2001. 
prossimo aggiornamento: europee 2024

Per vedere la lista completa degli anni/elezioni attualmente disponibili vedi [qui](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/dati_disponibili.xlsx)

## anteprima dati
Per avere un idea del tipo di dati messo a disposizione è disponibile un app che mostra un'anteprima dei risultati per le elezioni comunali 2016 e 2021. Per accedervi cliccare qui :https://gabrielepinto-dashboard-sezioni-elettorali-appstreamlite-4t5mbj.streamlit.app// (N.B. l'app mostra solo una parte dei risultati elettorali disponibili)

## shapefile
Gli shapefile che geolocalizzano le aree in cui sono localizzate le sezioni elettorali possono essere trovate sotto la cartella ![shapefiles sezioni elettorali](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali).
Per ogni comune, sono presenti due tipi di file: "precincts_voronoi" e "precincts_census". La differenza tra i due file è da ricondurre alle due diverse procedure utilizzate per ricostruire i poligoni nelle sezioni (a partire dai viari elettorali ufficiali forniti dai comuni). Entrambe le procedure sono descritte estensivamente in [questo paper](https://www.tandfonline.com/doi/full/10.1080/2474736X.2023.2185158). Alcuni comuni forniscono lo shapefile originale (es: Firenze e Genova) per questi comuni il nome del file è "precincts_original".  La lista completa può essere trovata nel file ![lista shapefile](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/anagrafica_shapefile.csv)

## risultati elettorali
I risultati elettorali coprono un periodo che va (circa) dal 2001 al 2022 (in costante aggiornamento) per varie tipologie di elezioni a seconda della disponibilità dei dati ufficiali che variano da comune a comune. L'archivio include i risultati a livello di sezione per referendum, voti di preferenza, elezioni sub-comunali (municipi, circoscrizioni, etc...), comunali, politiche, regionali, europee... tutti i file possono essere scaricati dall'archivio in formato rar che trovate ![qui](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/risultati_elettorali.rar): 
Per la lista della descrizione dei singoli file dei risultati elettorali consultare il file ![anagrafica completa](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/anagrafica_completa_all_cities.csv)
Per vedere la lista completa degli anni/elezioni attualmente disponibili vedi [qui](https://github.com/gabrielepinto/dati-sezioni-elettorali/raw/main/dati_disponibili.xlsx)
I dati contenuti nell'archivio sono il frutto di un lavoro di pulizia dei file originali disponibili nelle sezioni "open-data" dei vari comuni e possono essere facilmente "fusi" (merged) con gli shapefile utilizzando la chiave "SEZIONE" contenuta in tutti i file.

## dati censimento per sezione
La cartella  ![censimento sezioni elettorali](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/dati_censimento_sezione_elettorale) riporta per ogni citta il valore delle variabili censuarie ISTAT (1991,2001,2011) per ogni sezione elettorale calcolate con interpolazione spaziale. Oltre alle variabili standard fornite da ISTAT sono presenti anche una serie di indicatori (tasso di istruzione, cittadinanza etc...). La descrizione delle variabili è riportata nel file "tracciato_variabili.csv" [2011](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/dati_censimento_sezione_elettorale/tracciato_variabili_2011.csv),[2001](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/dati_censimento_sezione_elettorale/tracciato_variabili_2001.csv),[1991](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/dati_censimento_sezione_elettorale/tracciato_variabili_1991.csv).

## F.A.Q.

__per segnalare ulteriori F.A.Q. o segnalare errori/anomali nei dati aprire una ![issue](https://github.com/gabrielepinto/dati-sezioni-elettorali/issues) o scrivere a gabriele.pinto@uniroma1.it__

1. _Come posso aprire gli shapefile delle sezioni elettorali?_
Dopo aver scaricato gli shapefile dalla ![cartella](https://github.com/gabrielepinto/dati-sezioni-elettorali/tree/main/shapefiles_sezioni_elettorali) questi possono essere aperti e visualizzati utilizzando qualsiasi software GIS open-source (es: ![QGIS](https://qgis.org/en/site/forusers/download.html)) o a pagamento in grado di aprire i file di tipo [ESRI shapefile](https://en.wikipedia.org/wiki/Shapefile).
In alternativa, gli shapefile possono essere letti "online" effettuando una richiesta direttamente al repository. Per un esempio con Python vedere ![questo notebook di esempio](https://github.com/gabrielepinto/dati-sezioni-elettorali/blob/main/esempio_apertura_file.ipynb).

2. _A quale versione del viario elettorale corrispondono le sezioni elettorali?_  
L'ultima disponibile. Generalmente, Settembre 2021. 

3. _Qual'è la fonte dei risultati elettorali ?_ 
La fonte sono le sezioni open-data dei comuni italiani. Poichè i comuni forniscono in dati in formati non inter-operabili questi sono stati "puliti" tramite varie procedure e ricondotti in unici file per ogni elezione. Ad esempio, l'archivio online del  [comune di roma](https://www.elezioni.comune.roma.it/archivio.asp) con i risultati elettorali a livello di sezione contiene oltre 5000 file excel (un file per ogni lista, etc...) che seguono (spesso) formattazioni diverse. Questi sono stati ricondotti ad un unico file per ogni elezione per aumentarne la fruibilità. Ragionamenti simili valgono per i comuni di [Torino](http://aperto.comune.torino.it/dataset?dcat_subtheme_it=0416+procedura+elettorale+e+voto) e [Milano](https://dati.comune.milano.it/dataset?tags=elezione)

4. _Come è calcolata l'AFFLUENZA ?_ 
Per alcune città/round di elezioni i voti __nulli/bianchi/contestati__ non sono disponibili, ai fini di garantire omogeneità l'affluenza (colonna "AFFLUENZA") è sempre calcolata come somma del totale dei __voti validi__ (colonna "TOTALE") sul totale degli iscritti alla sezione in quell'anno. 

5. _Perchè in alcune sezioni il valore dell'affluenza riporta dei valori anomali (es: maggiore di 1 o infinito)_?
Per due motivi prevalenti:
    1. sezioni speciali (ad es: seggi speciali come ospedali, caserme etc... dove non ci sono "iscritti")
    2. errore materiale nell'archivio del comune (frequenti)

6. _Quando verranno resi disponibili i dati di nuove città?_
a mano a mano che vengono ottenuti i viari elettorali (necessari al fine di costruire i poligoni delle sezioni).

7. _Come vengono implementate le procedure/algoritmi  descritti nel  [paper](https://www.tandfonline.com/doi/full/10.1080/2474736X.2023.2185158) ?_
Le due procedure sono state codificate in Python e possono essere celermente applicate direttamente al viario elettorale di qualsiasi città.

8. _Si possono coprire tutte le città di Italia con questa procedura?_
In teoria si...se fossero disponibili tutti i viari elettorali di tutti i (quasi 8000) comuni Italiani. Nella pratica, raccogliere tutti i viari elettorali dei comuni italiani è impresa ardua. D'altra parte, il valore informativo di questo tipo di dettaglio è rilevante solo per i comuni sopra determinate soglie dimensionali (es: con + di 20/30 sezioni - 15.000 abitanti - circa 500 comuni)

9. _Perchè è tutto in italiano_ ?
a breve pubblicheremo una versione inglese del readme

10. _Esiste una classificazione dei partiti/candidati/liste ?_
Si, a breve verrà pubblicato un file con una classificazione _grossolana_ dei candidati/partiti/liste per coalizioni di destra/sinistra/altro.

11. _Posso unire i dataset con altre fonti (es: manifesto project, CLEA, anagrafe amministratori, etc...) ?_ 
Al momento il procedimento non è così automatico per due motivi:
    1. Molti candidati/partiti/liste che partecipano alle elezioni locali non sono presenti nei principali dataset internazionali.
    2. I nomi dei candidati/partiti/liste non sono codificati in modo omogeneo (es: in un dataset ci può essere "PARTITO DEMOCRATICO", in altro "P.DEMOCRATICO"....etc..). Per ora sono stati lasciati così per rendere più facile rintracciare eventuali errori nella fase di pulizia del dato.

12. _Il ministero dell'interno (DAIT-ELIGENDO) non raccoglie i dati a livello di sezione elettorale?_
Secondo la risposta di un accesso civico il ministero dell'interno sta sperimentando la raccolta dei dati a livello di sezione elettorale. Quando e se questi dati verranno resi disponibili sarà più facile "fondere" gli shapefile con i risultati.
