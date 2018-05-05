## Algoritmo di scelta

La fase 2 tiene conto di tutti i requisiti (vedi p. 16: "eventuali costi di
personalizzazione, necessari ad assicurare la copertura di *tutti* i requisiti
funzionali e non funzionali, indispensabili e non indispensabili").

La fase 3, invece:

  1. tiene conto di tutti i requisiti per la realizzazione ex-novo (vedi p.
  19: 
  > "La Pubblica amministrazione, dopo aver individuato l’esistenza o meno di
  una soluzione proprietaria confacente ai propri bisogni, elabora un documento
  contenente un progetto di fattibilità contenente la stima delle attività, dei
  costi e dei tempi da sostenere per la realizzazione di una soluzione ex-novo
  che *soddisfi completamente le esigenze* indicate nel documento sull’analisi
  dei fabbisogni così come descritto nella “Fase 1.1: Analisi del
  fabbisogno”."), e
  2. non tiene conto di tutti i requisiti per il software proprietario (vedi p. 19:
  > "assicurare la soddisfazione dei requisiti funzionali e non determinati
  nella Macro fase 1, garantendo il *soddisfacimento di quelli
  indispensabili*, con quelli indicati nella documentazione").

Apparentemente, questo algoritmo può essere aggirato facilmente: è sufficiente prevedere
nella fase 1 dei requisiti non indispensabili che non sono disponibili in
nessuna soluzione in riuso e software libero per passare serenamente alla fase 3
saltando la 2 e quindi preferire software proprietario (che non deve soddisfare
tutti i requisiti). C'è qualcosa da correggere. Per esempio, si può prevedere
che se non esiste una soluzione proprietaria con tutti i requisiti previsti
nella fase 1, si riapre la fase 2 valutando solo i requisiti indispensabili per
software in riuso e software libero. Oppure si chiarisce che la valutazione make riguarda
anche il caso in cui si personalizza del software in riuso o software libero e, in questa
fase, la valutazione si può limitare ai requisiti soddisfatti dalla migliore
soluzione proprietaria.

### Manca una subfase: marginale integrazione del software

Nell'ottica del commento precedente, non pare corretto arrestare la valutazione
dei requisiti mancanti di un progetto in riuso o di software libero senza tener conto
della possibilità di **integrare** il requisito mancante con una minima o
comunque non dispendiosa modifica, eventualmente da mandare "_upstream_" una
volta implementata.

A differenza di quanto avviene nel mondo proprietario, infatti, le soluzioni di
software libero e in riuso non sono necessariamente da prendere a scatola chiusa, ma
concedono il diritto a chiunque di modificare il codice per adattarlo. Se quanto
manca è ad esempio un connettore con una banca dati, ma l'infrastruttura
consente di crearle, questa è una modifica banale e rigettare un progetto software
libero solo perché non ha quella funzionalità non fa un servizio alla
collettività.

D'altronde molte acquisizione di software anche proprietario includono una fase
di **manutenzione evolutiva** per ad esempio adattare il software alle esigenze
di mutate normative. Dunque molte acquisizioni di software in realtà hanno
incorporato anche una non preponderante fase di sviluppo. È nostro parere che
una soluzione in riuso o di software libero in questo caso rimanga nella rispettiva
categoria anche se include una limitata fase di adattamento. Dunque la
valutazione non deve essere fatta in modo "binario", ma adottando una logica di
prossimità/lontananza dalla soluzione auspicata. D'altronde, aggiungendo una
parte "_make_" il software rimane sempre software in riuso/soggetto a
riuso/software libero, qualsiasi combinazione di elementi si consideri.

### Gerarchia tra subfasi di valutazione software libero e software in riuso risulta arbitraria

L'art. 68 comma 1-ter CAD in realtà non opera distinzioni tra queste due
categorie e le pone allo stesso ordine di preferenza. Nemmeno un criterio
semantico porta a considerare una soluzione privilegiata rispetto all'altra.
Nonostante "software liberi..." (sic) sia un inciso, "adeguati" si riferisce a
tutti i casi trattati nel comma.

Inoltre, visto che l'art. 69 prevede comunque il rilascio del codice in forma
pubblica con una licenza libera, si può ragionevolmente sostenere che tutto il
software in riuso sia anche software libero. Pertanto non si comprende perché
una volta che vi siano soluzioni _sia_ di software libero _sia_ di software in
riuso, non si debba procedere a una valutazione comparativa rispetto a queste
categorie, senza fermarsi a quella in riuso, se quella in software libero fosse
più adatta e complessivamente migliore, al di là della titolarità in capo a una
pubblica amministrazione. Ad esempio, quella in software libero potrebbe avere una
comunità più viva, oppure essere basata su un middleware o un'infrastruttura
uguale a quella già adottata dalla PA, eccetera. Privarsi di questa possibilità
in assenza di una norma che lo preveda espressamente pare non essere in linea
con i dettami normativi.

Si suggerisce che il fatto di trovare una soluzione in riuso potenzialmente
adeguata non sia un punto di uscita dall'albero decisorio, ma dia comunque come
esito il passaggio alla valutazione successiva, dovendosi ricercare se non vi
siano soluzioni in software libero utilizzabili anche non appartenenti al dominio del
riuso, per poi operare una valutazione comparata se più soluzioni passino l'uno
o l'altro filtro.

## Responsabilità

Si ritiene che vada posta più attenzione al tema della compliance per chi riusa.

Soprattutto se:

   1. chi riusa distribuisce il software, o
   2. il software che si riusa (o le dipendenze di questo) sono disponibili
   secondo i termini di licenze network copyleft.

Ma il problema della compliance va gestito anche se non ci sono licenze
copyleft: mantenere le copyright notices, accompagnare il codice con il
testo delle licenze quando è richiesto, ecc.. Si tenga conto del fatto che
qualsiasi attività di realizzazione di software soggetto a riuso determina
obbligatoriamente una distribuzione. Pertanto, quando si commissiona software
sviluppato ad hoc, poiché inevitabilmente questo comporterà l'utilizzo di
componenti di terze parti, occorre che il software "_inbound_" abbia condizioni
di licenza o di titolarità compatibili con la licenza del software in uscita.

Chi riusa e chi realizza software in riuso si dovranno porre il problema della compliance e le linee guida
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
e 69 (questo è un problema delle norme, non delle linee guida) ma, anche
senza intervenire sulle norme, si potrebbero costruire policy, incentivi
e pratiche che favoriscono la collaborazione tra le PA per sviluppare e
distribuire software libero utile a molte PA.
