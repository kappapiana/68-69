## Algoritmo di scelta

### Relazione tra le subfasi della fase 2

L'art. 68 comma 1-ter CAD in realtà non opera distinzioni tra la 
categorie del software in riuso e il software libero e le pone allo stesso ordine di preferenza. 
Nemmeno un criterio semantico porta a considerare una soluzione privilegiata rispetto all'altra: 
il termine "adeguati" utilizzato nel comma 1 si riferisce a 
tutti i casi trattati nel comma stesso.

Ove vi siano soluzioni _sia_ di software libero _sia_ di software in
riuso, pare utile procedere a una valutazione comparativa rispetto a queste
categorie, senza fermarsi a quella in riuso, se quella in software libero fosse
più adatta e complessivamente migliore. Ad esempio, quella in software libero potrebbe avere una
comunità più viva, oppure essere basata su un middleware o un'infrastruttura
uguale a quella già adottata dalla PA, eccetera. Privarsi di questa possibilità
in assenza di una norma che lo preveda espressamente è illegittimo in quanto contraddice 
i principi di economicità e di efficienza previsti al comma 1.

Si suggerisce che il fatto di individuare una soluzione in riuso potenzialmente
adeguata non sia un punto di uscita dall'albero decisorio, ma dia comunque come
esito il passaggio alla valutazione successiva, dovendosi ricercare se non vi
siano soluzioni in software libero utilizzabili anche non appartenenti al dominio del
riuso, per poi operare una valutazione comparata se più soluzioni passino l'uno
o l'altro filtro.

### Relazione tra la fase 2 e la fase 3

La fase 2 tiene conto di tutti i requisiti; a p. 16 delle Linee Guida si legge che
  > "eventuali costi di
personalizzazione, necessari ad assicurare la copertura di **tutti** i requisiti
funzionali e non funzionali, indispensabili e non indispensabili").

La fase 3, invece:

  1. tiene conto di tutti i requisiti per la realizzazione ex-novo; infatti a p.
  19 si legge
  > "La Pubblica amministrazione, dopo aver individuato l’esistenza o meno di
  una soluzione proprietaria confacente ai propri bisogni, elabora un documento
  contenente un progetto di fattibilità contenente la stima delle attività, dei
  costi e dei tempi da sostenere per la realizzazione di una soluzione ex-novo
  che **soddisfi completamente le esigenze** indicate nel documento sull’analisi
  dei fabbisogni così come descritto nella “Fase 1.1: Analisi del
  fabbisogno”."
  2. non tiene conto di tutti i requisiti per il software proprietario; infatti a p. 19 si legge
  > "assicurare la soddisfazione dei requisiti funzionali e non determinati
  nella Macro fase 1, garantendo il **soddisfacimento di quelli indispensabili**, 
  con quelli indicati nella documentazione".

Apparentemente, questo algoritmo può essere aggirato facilmente: è sufficiente prevedere
nella fase 1 dei requisiti non indispensabili che non sono disponibili in
nessuna soluzione in riuso e software libero per passare serenamente alla fase 3
saltando la 2 e quindi preferire software proprietario (che non deve soddisfare
tutti i requisiti). C'è qualcosa da correggere. Per esempio, si può prevedere
che se non esiste una soluzione proprietaria con tutti i requisiti previsti
nella fase 1, si riapre la fase 2 valutando solo i requisiti indispensabili per
software in riuso e software libero. Oppure si chiarisce che la valutazione _make_ della fase 3 
è limitata ai soli requisiti soddisfatti dalla migliore soluzione proprietaria e riguarda
anche il caso in cui si personalizza del software in riuso o software libero.

## Responsabilità

Si ritiene che vada posta più attenzione al tema della valutazione di conformità legale.

Qualsiasi attività di realizzazione di software soggetto a riuso determina
obbligatoriamente una distribuzione. Pertanto, quando si commissiona software
sviluppato _ad hoc_ che comporti l'utilizzo di 
componenti di terze parti, occorre che il software "_inbound_" abbia condizioni
di licenza o di titolarità compatibili con la licenza del software in uscita. 
Si suggerisce di prevedere che i contratti di appalto tengano conto di quanto sopra, 
obbligando il fornitore a svolgere la valutazione di conformità ed a documentarne gli esiti 
alla PA appaltante.

Anche chi riusa il software deve svolgere una valutazione di conformità, soprattutto se:

   1. chi riusa distribuisce il software, o
   2. il software che si riusa (o le dipendenze di questo) sono disponibili
   secondo i termini di licenze network copyleft.

Ma il problema della valutazione di conformità legale va gestito anche se non ci sono licenze
copyleft. È necessario mantenere le copyright notices, accompagnare il codice con il
testo delle licenze quando è richiesto, ecc.. 

Chi realizza software che viene rilasciato in riuso e chi riusa si deve porre il problema 
della valutazione di confomità legale e le Linee Guida
dovrebbero dirlo chiaramente.

Si ritiene anche utile indirizzare gli enti a risorse di supporto nella
realizzazione della valutazione e delle azioni da intraprendere (tools,
specifiche come [Openchain](https://openchainproject.org), ecc.).  

Forse potrebbe essere utile prevedere una sorta di "certificazione": se
una PA svolge l'analisi, potrebbe documentare gli esiti della stessa
analisi (nel portale developers?) perché siano disponibili alle altre
PA.

## Mutualizzazione dei costi

Riteniamo che un generico invito alle PA a collaborare per mettere a fattor
comune scelte di sviluppo e licenza di nuove soluzioni sarebbe utile.
Ci rendiamo conto che non è un risultato che può discendere dagli artt. 68
e 69 (questo è un problema delle norme, non delle Linee Guida) ma, anche
senza intervenire sulle norme, si potrebbero costruire policy, incentivi
e pratiche che favoriscono la collaborazione tra le PA per sviluppare e
distribuire software libero utile a molte PA.
