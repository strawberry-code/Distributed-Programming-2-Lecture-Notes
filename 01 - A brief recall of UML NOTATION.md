# A brief recall of UML NOTATION



## Lesson outline

1. Class Diagrams
2. Package Diagrams
3. Object Diagrams
4. Sequence Diagrams



## Richiami su UML

In ingegneria del software, **UML** (unified modeling language, *"linguaggio di modellizzazione unificato"*) è un linguaggio di modellizzazione e specifica basato sul paradigma orientato agli oggetti. Il nucleo del linguaggio fu definito nel 1996 da Grady Booch, Jim Rumbaugh e Ivar Jacobson (detti *"i tre amigos"*) sotto l'egida dell'*Object Management Group*, consorzio che tuttora gestisce lo **standard UML**. Il linguaggio nacque con l'intento di unificare approcci precedenti (dovuti ai tre padri di UML e altri), raccogliendo le migliori prassi nel settore e definendo così uno standard industriale unificato.

L'UML svolge un'importantissima funzione di "**lingua franca**" nella comunità della progettazione e programmazione a oggetti. Gran parte della letteratura di settore usa UML per descrivere soluzioni analitiche e progettuali in modo *sintetico* e *comprensibile* a un vasto pubblico.

L'ultima versione del linguaggio, la **2.0**, è stata consolidata nel 2004 e ufficializzata da OMG nel 2005. UML 2.0 riorganizza molti degli elementi della versione precedente (1.5) in un quadro di riferimento ampliato e introduce molti nuovi strumenti, inclusi alcuni nuovi tipi di diagrammi. Sebbene OMG indichi UML 2.0 come la versione "corrente" del linguaggio, la transizione è di fatto ancora in corso; le stesse specifiche pubblicate da OMG sono ancora non completamente aggiornate e il supporto dei tool a UML 2.0 è, nella maggior parte dei casi, appena abbozzato.



## Class Diagrams

I **diagrammi delle classi** (*class diagram*) sono uno dei tipi di diagrammi che possono comparire in un modello UML. In termini generali, consentono di descrivere tipi di entità, con le loro caratteristiche e le eventuali relazioni fra questi tipi. Gli strumenti concettuali utilizzati sono il concetto di classe del paradigma *object-oriented* e altri correlati (per esempio la **generalizzazione**, che è una relazione concettuale assimilabile al meccanismo object-oriented dell'**ereditarietà**).

##### Usi dei diagrammi delle classi

Uno degli assunti fondamentali del paradigma a oggetti è che il concetto di classe, e concetti correlati come l'ereditarietà o il polimorfismo, si prestino a rappresentare in modo diretto e intuitivo la realtà, in qualsiasi ambito (per usare le parole di Grady Booch, "un oggetto è qualsiasi cosa a cui si possa pensare"). I diagrammi delle classi UML sono basati su versioni astratte di tali concetti, e possono essere utilizzati per descrivere sostanzialmente qualsiasi contesto a qualsiasi livello di astrazione (enfatizzandone, però, solo alcuni aspetti). Di conseguenza, UML prevede un loro impiego a livello di analisi e in particolare analisi del dominio (ovvero la descrizione del contesto in cui un sistema software deve operare), ma anche a livello di progettazione (nella descrizione della struttura interna del sistema, dei suoi componenti e delle loro relazioni).



#### Concetti principali

##### Classe

L'elemento di modello principale dei diagrammi delle classi è la classe. Una classe rappresenta una categoria di entità (istanze), nel caso particolare dette oggetti; il nome della classe indica la categoria di entità descritta dalla classe. Ogni classe è corredata da un insieme di attributi (che descrivono le caratteristiche o lo stato degli oggetti della classe) e operazioni (che descrivono il comportamento della classe). Il simbolo grafico che rappresenta le classi UML è un rettangolo suddiviso in tre scomparti, rispettivamente dedicati al nome della classe, agli attributi e alle operazioni.



##### Relazione

Due classi possono essere legate da relazioni che rappresentano i legami (link) che possono sussistere fra gli oggetti delle classi associate. Tali Relazioni possono essere corredate da un insieme di informazioni aggiuntive, per esempio, il ruolo svolto da ogni classe o la molteplicità della relazione (il numero di oggetti delle due classi che possono essere coinvolti in un link). Esistono diversi tipi di relazione (associazione, aggregazione, composizione, dipendenza, generalizzazione, realizzazione), e ogni tipo viene rappresentato mediante una particolare linea orientata da una freccia che connette le due classi coinvolte.



##### Associazione

Due classi possono essere legate da relazione di associazione, che indica che gli oggetti delle due classi condividono una relazione statica.



##### Dipendenza

Due classi possono essere legate da una relazione di dipendenza, che indica che la definizione di una delle due fa riferimento alla definizione dell'altra.



##### Generalizzazione

Due classi possono essere legate da una relazione di generalizzazione, che indica che una delle due classi (detta superclasse) si può considerare una generalizzazione dell'altra (detta sottoclasse).



##### Esempio di diagramma

Esempio di *Class Diagram*:

![alt text](immagini/lezione-01/01.png)

Il diagramma descrive due entità (i rettangoli), Cliente e Reclamo, e le relative relazioni (il segmento che li unisce).

Il nome della **classe** è riportato come nome del rettangolo che compare nella parte superiore dello stesso. Gli **attributi**, o caratteristiche del cliente, compaiono nella parte centrale del rettangolo e in questo caso rispetto alla Classe Cliente sono un identificativo, il cognome, il nome ed il telefono (si descrivono solo gli attributi utili al modello).

I comportamenti, o **metodi**, compaiono nella parte inferiore del rettangolo e relativamente alla classe Reclamo, sono le azioni Crea, Modifica o Chiudi.

La relazione indica anche una **cardinalità** (i numeri posti vicino alle Classi) del tipo 1 a molti e in questo caso si leggono "ad 1 Cliente corrispondono 1 o n Reclami" e "ad 1 Reclamo corrisponde 1 Cliente".



##### Interfacce

Nel modellamento UML, le interfacce sono elementi di modello che definiscono serie di operazioni che altri elementi, ad esempio le classi, o componenti devono implementare. Un elemento del modello di implementazione realizza un'interfaccia sostituendo ogni operazione dichiarata dall'interfaccia.

È possibile utilizzare le interfacce nei diagrammi di classe e di componente per specificare un accordo tra l'interfaccia e il classificatore che la realizza. Ogni interfaccia specifica una serie ben definita di operazioni con visibilità pubblica. Le firme dell'operazione indicano ai classificatori di implementazione il tipo di funzionalità da richiamare, ma non come eseguire tale operazione. Diversi classificatori possono implementare una singola interfaccia, ognuno fornendo un'implementazione univoca.

Le interfacce supportano la non visualizzazione di informazioni e la protezione del codice client tramite dichiarazione pubblica di determinati servizi e funzionalità. Le classi o i componenti che realizzano le interfacce implementando tale funzionalità semplificano lo sviluppo di applicazioni, perché gli sviluppatori che scrivono il codice client devono conoscere solo le interfacce e non i dettagli dell'implementazione. Se si sostituiscono le classi o i componenti che implementano le interfacce, nel modello non è necessario progettare di nuovo l'applicazione se i nuovi elementi di modello implementano le stesse interfacce.

Le interfacce si identificano nel seguente modo: `<<interface name>>`.



## Package Diagrams

Un package nell'Unified Modeling Language è usato *"per raggruppare elementi e fornire un namespace per gli elementi raggruppati"*. Un package può contenere altri package, fornendo così un'**organizzazione gerarchica** dei package.

Praticamente *tutti gli elementi UML possono essere raggruppati in package*. Così classi, oggetti, use case, componenti, nodi, istanze di nodi, ecc. possono essere tutti organizzati come package, consentendo così una maneggevole organizzazione delle miriadi di elementi che un modello UML comporta.

##### Utilizzo

Quando si organizzano modelli funzionali (use case, workflow, ecc.) si usano i package per modellare la struttura modulare del sistema da applicare nel mondo reale. Quando si organizza il codice sorgente, si usano i package per rappresentare i differenti strati di un codice sorgente. 

Un esempio di package diagram:




## Object Diagrams



## Sequence Diagrams