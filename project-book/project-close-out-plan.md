# Data project retrospective

{% hint style="danger" %}
_Crea: PM  
Aiuta: TL, DS, DA  
Revisiona: HoPM, HoDS, HoDA  
Informato:_
{% endhint %}

{% hint style="info" %}
_Questa sezione viene compilata in due fasi di progetto:_

* _**Durante il progetto**: Al termine di ogni macro attività è possibile effettuare una **analisi delle criticità**, individuando quali sono i **rischi** da valutare se si dovesse intraprendere nuovamente una commessa simile._
* _**A valle del progetto**: In questa fase si ha la vera e propria **analisi retrospettiva**, nella quale si effettua uno studio **SWOT**, si analizza quanto ci si è discostati dai **goals definiti a inizio progetto** e si analizza lo **scostamento del preventivo dal consuntivo** in termini di tempi e costi._

_La analisi retrospettiva, oltre a formare il team e prepararlo a successive commesse con una lesson learned, fornisce informazioni al **team innovation** in ottica di creazione di **servizi prodottizzati** derivanti dalle attività della commessa._
{% endhint %}

{% file src="../.gitbook/assets/modern-data-project-retrospective.pdf" caption="Data project retrospective" %}

## _SWOT_

{% tabs %}
{% tab title="Strenghts" %}

{% endtab %}

{% tab title="Weakness" %}

{% endtab %}

{% tab title="Opportunities" %}

{% endtab %}

{% tab title="Threats" %}

{% endtab %}
{% endtabs %}

## Analisi consuntivo

|  | Pianificati | Effettivi |
| :--- | :--- | :--- |
| **Tempi** |  |  |
| **Costi** |  |  |

## Appunti su criticità

### Raccolta dati:

* Accesso ai dati tramite VPN e collegamento al DB del loro gestionale di produzione \(NICIM\) 
* Integrazioni \(specifiche tecniche delle macchine di produzione\) con file Excel 

Criticità:

* Elevato numero di tabelle e viste presenti \(molte vuote\); poca chiarezza su quelle effettivamente necessarie 
* Nomi delle colonne non sempre esplicativi delle variabili rappresentate \(es: diversi tipi di tempi avviamento e tempi preparazione\) 
* Necessità di spiegazioni da parte del cliente riguardo al significato delle colonne del DB e di quali tabelle \(viste\) tener conto 

### Validazione dati:

* Client VPN, SQLDeveloper, Jupyter \(Pandas, Pyvis, Plotly, …\) 
* Variabili necessarie: Codice articolo, Codice stampo, Codice pressa, Velocità di produzione\(bt/h\), Tempi di preparazione per cambio stampo \(h\), Tempi di preparazione per cambio tasselli \(h\), Associazione bolla madre-bolle figlie   

Criticità dati:

* Codice stampo indicato dal cliente, non immediato da riconoscere interpretando il nome della colonna nel DB 
* Necessaria spiegazione da parte del cliente sulle molteplici velocità di produzione storicizzate e sul loro utilizzo \(velocità prevista, velocità effettiva, velocità effettiva al netto di fermi/scarti\) 
* Lo stesso dicasi per i tempi di preparazione \(tempi avviamento, tempo preparazione, tempo montaggio, tempi di fermo, tempo consuntivato, …\) 
* Distinzione tra bolle cucite e tasselli non ben definita anche dopo l’analisi delle tabelle \(probabilmente dovuto a come il cliente storicizza i dati\) 

Criticità analisi:

* Nessuna particolare criticità riscontrata a livello tecnico 
* È stata molto utile la funzione di integrazione di query SQL a livello di linguaggio Python in Jupyter  

## Matrice Polipo

In quest'area, si richiede al _PM_ di compilare la seguente tabella al fine di integrare le informazioni nella [matrice Polipo](https://energywaysrlit.sharepoint.com/:x:/s/EnergyWay/EbRHJq41-VlKhyZ7FdD96VYBqCQNCeiWdg9AU3rwKluxdg?e=qvhF6z), strumento di studio comparato e strategico delle commesse.

La compilazione dovrà avvenire \(o essere ultimata\) **al termine del progetto**.

| Colonne matrice | Contenuto |
| :--- | :--- |
| **User** | - |
| **Servizio/prodotto** | - |
| **Value Proposition** | - |
| **Performance vs Benchmark** | - |
| **Analisi dei competitor \(e.g. internazionalizzazione, go-to-market\)** | - |
| **Gap analysis tecnica per industrializzare la soluzione** | - |
| **Criticità** | - |
| **Spunti per l'industrializzazione di casi simili** | - |

Una volta compilata o aggiornata la tabella, integrare i dati all'interno del file excel.

