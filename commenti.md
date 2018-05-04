## Algoritmo di scelta

La fase 2 tiene conto di tutti i requisiti (vedi p. 16: "eventuali costi di
personalizzazione, necessari ad assicurare la copertura di *tutti* i requisiti
funzionali e non funzionali, indispensabili e non indispensabili").

La fase 3, invece:

  1. tiene conto di tutti i requisiti per per la realizzazione ex-novo (vedi p.
  19: "La Pubblica amministrazione, dopo aver individuato l’esistenza o meno di
  una soluzione proprietaria confacente ai propri bisogni, elabora un documento
  contenente un progetto di fattibilità contenente la stima delle attività, dei
  costi e dei tempi da sostenere per la realizzazione di una soluzione ex-novo
  che *soddisfi completamente le esigenze* indicate nel documento sull’analisi
  dei fabbisogni così come descritto nella “Fase 1.1: Analisi del
  fabbisogno”."), e
  2. non tiene conto di tutti i requisiti per il sw proprietario (vedi p. 19:

> "assicurare la soddisfazione dei requisiti funzionali e non determinati
nella Macro fase 1, garantendo il *soddisfacimento di quelli
indispensabili*, con quelli indicati nella documentazione").

IMHO questo algoritmo può essere aggirato facilmente: è sufficiente prevedere
nella fase 1 dei requisiti non indispensabili che non sono disponibili in
nessuna soluzione in riuso e sw libero per passare serenamente alla fase 3
saltando la 2 e quindi preferire un sw proprietario (che non deve soddisfare
tutti i requisiti). C'è qualcosa da correggere. Per esempio, si può prevedere
che se non esiste una soluzione proprietaria con tutti i requisiti previsti
nella fase 1, si riapre la fase 2 valutando solo i requisiti indispensabili per
sw in riuso e sw libero. Oppure si chiarisce che la valutazione make riguarda
anche il caso in cui si personalizza del sw in riuso o sw libero e, in questa
fase, la valutazione si può limitare ai requisiti soddisfatti dalla migliore
soluzione proprietaria.

## Responsabilità

Penso vada posta più attenzione al tema della compliance per chi riusa.

Soprattutto se:

   1. chi riusa distribuisce il sw, o
   2. il sw che si riusa (o le dipendenze di questo) sono disponibili
   secondo i termini di licenze network copyleft.

Ma il problema della compliance va gestito anche se non ci sono licenze
copyleft: mantenere le copyright notices, accompagnare il codice con il
testo delle licenze quando è richiesto, ecc..

Chi riusa si deve porre il problema della compliance e le linee guida
dovrebbero dirlo.

Penso sia anche utile indirizzare gli enti a risorse di supporto nella
realizzazione della valutazione e delle azioni da intraprendere (tools,
specifiche come [Openchain](https://openchainproject.org), ecc.).  

Forse potrebbe essere utile prevedere una sorta di "certificazione": se
una PA svolge l'analisi, potrebbe documentare gli esiti della stessa
analisi (nel portale developers?) perché siano disponibili alle altre
PA.

## Mutualizzazione dei costi

Credo che un generico invito alle PA a collaborare per mettere a fattor
comune scelte di sviluppo e licenza di nuove soluzioni sarebbe utile.
Mi rendo conto che non è un risultato che può discendere dagli artt. 68
e 69 (questo è un problema delle norme, non delle linee guida) ma, anche
senza intervenire sulle norme, si potrebbero costruire policy, incentivi
e pratiche che favoriscono la collaborazione tra le PA per sviluppare e
distribuire sw libero utile a molte PA.
