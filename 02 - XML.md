# 02 - XML

XML (sigla di eXtensible Markup Language) è un metalinguaggio per la definizione di linguaggi di markup, ovvero un linguaggio marcatore basato su un meccanismo sintattico che consente di definire e controllare il significato degli elementi contenuti in un documento o in un testo.

Costituisce il tentativo di produrre una versione semplificata di Standard Generalized Markup Language (SGML) che consente di definire nuovi linguaggi di markup.

Il nome indica che si tratta di un linguaggio marcatore (markup language) estensibile (eXtensible) in quanto permette di creare tag personalizzati.



## Gli standard per lo scambio di dati in ambienti distribuiti

Ci sono degli standard che definiscono dei linguaggi che possono essere utilizzati per lo scambio di dati. Si tratta perlopiù di linguaggi che definiscono files o strutture dati in formati aperti (open formats), cioè sono *neutrali* e indipendenti dai sistemi.

Le due principali caratteristiche di ciascuno di questi standard sono:

1. essere un linguaggio in grado di definire **tipi di dati astratti**,
2. **rappresentare i dati in modo neutrale** cioè, come detto, indipendenti dai sistemi con i quali stanno interagendo.

Lo scambio di dati può avvenire, per esempio, tra un server basato su Java Spring e un client basato su JavaScript e i dati sono codificati tramite **JSON**. Tra le due piattaforme ci sarà un minimo di elaborazione per la *codifica/decodifica* di tali dati.

Di questi standard citiamo:

- **ASN-1** - Abstract Syntax Notation One e indica un linguaggio astratto che può essere usato per descrivere una notazione, le relative procedure di encoding e il software che viene utilizzato per maneggiare il codice. È stato definito nel 1990 nello standard ISO 8824 e ripreso nel 2000.

- **XDR** - Sviluppato nella metà del 1980 da Sun Microsystems e pubblicato per la prima volta nel 1987. È diventato uno standard IEFT nel 1995.

- **COBRA CDR** - Common Data Representation (CDR) viene utilizzato per rappresentare dati strutturati o primitivi che vengono passati come argomenti o come valori di ritorno durante le invocazioni remote negli oggetti distribuiti CORBA (Common Object Request Broker Architecture).

  Permette la comunicazione tra client e server che sonos tati scritti in linguaggi differenti tra loro. Per esempio, può tradurre in little-endian in big-endian e viceversa. 

- **XML** -  È un metalinguaggio per la definizione di linguaggi di markup, ovvero un linguaggio marcatore basato su un meccanismo sintattico che consente di definire e controllare il significato degli elementi contenuti in un documento o in un testo.

- **JSON** -  Acronimo di JavaScript Object Notation, è un formato adatto all'interscambio di dati fra applicazioni client-server.

  È basato sul linguaggio JavaScript Standard ECMA-262 3ª edizione dicembre 1999, ma ne è indipendente. Viene usato in AJAX come alternativa a XML/XSLT.

In particolare **XML** e **JSON** sono quelli che attualmente stanno avendo larga diffusione e grande popolarità.



## Principali caratteristiche di XML



## XML (eXtensible Markup Language)



### SGML



#### Terminologia SGML



### Esempio di riferimento a un documento HTML (DTD)



### Relazioni tra SGML, HTML e documenti XML



## Un semplice documento XML



## Schema concettuale di un documento XML



### Organizzazione logica di un documento XML



### Organizzazione fisica di un documento XML



### Sintassi generale di un documento XML



### Strutture sintattiche XML



### Markups specifici di XML

#### Le dichiarazioni XML

#### Le dichiarazioni DTD



### Validità di un documento XML



## DTD



### Esempio di DTD



### Dichiarazione di un elemento



### Modelli di elementi



### Esempi di modelli di elementi



### Mixed models



### Dichiarazione di un attributo



### Specificare il tipo dei valori



### Significato dei vari tipi di *tokens*



### Dichiarazioni di default



### Esempio



## Esercizio



## Come viene processato un documento XML?

 ### Schema di processamento di un documento XML



## Document Object Model (DOM)

### Organizzazione delle specifiche del DOM

### Interfacce DOM di livello 1

### L'elemento <\<interface>>



## Semplici API per XML (SAX)



## API di tipo streaming per XML (StAX)



## Confronto tra DOM/SAX/StAX



## Presentazione di un documento XML



## XSL: eXtensible Stylesheet Language

### Esempio di XSL



## XSLT

### Esempio di XSLT