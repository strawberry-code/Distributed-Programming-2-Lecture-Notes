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



## XML (eXtensible Markup Language)

In informatica XML (sigla di eXtensible Markup Language) è un metalinguaggio per la definizione di linguaggi di markup, ovvero un linguaggio marcatore basato su un meccanismo sintattico che consente di definire e controllare il significato degli elementi contenuti in un documento o in un testo.

Costituisce il tentativo di produrre una versione semplificata di Standard Generalized Markup Language (SGML) che consente di definire nuovi linguaggi di markup, dal quale – appunto – deriva.

Il nome indica che si tratta di un linguaggio marcatore (markup language) estensibile (eXtensible) in quanto permette di creare tag personalizzati.



### Storia

Il World Wide Web Consortium (W3C), in seguito alla guerra dei browser (ovvero la situazione verificatasi negli anni novanta nella quale Microsoft e Netscape introducevano, con ogni nuova versione del proprio browser, un'estensione proprietaria all'' HTML ufficiale), fu costretto a seguire le individuali estensioni al linguaggio HTML.

Il W3C dovette scegliere quali caratteristiche standardizzare e quali lasciare fuori dalle specifiche ufficiali dell'HTML. Fu in questo contesto che iniziò a delinearsi la necessità di un linguaggio di markup che desse maggiore libertà nella definizione dei tag, pur rimanendo in uno standard.

Il "progetto XML", che ebbe inizio alla fine degli anni novanta nell'ambito della SGML Activity del W3C, suscitò un così forte interesse che la W3C creò un gruppo di lavoro, chiamato XML Working Group, composto da esperti mondiali delle tecnologie SGML, ed una commissione, XML Editorial Review Board, deputata alla redazione delle specifiche del progetto.

Nel febbraio del 1998 le specifiche divennero una raccomandazione ufficiale con il nome di Extensible Mark-up Language, versione 1.0. Ben presto ci si accorse che XML non era limitato al solo contesto web ma era qualcosa di più: uno strumento che permetteva di essere utilizzato nei più diversi contesti, dalla definizione della struttura di documenti, allo scambio delle informazioni tra sistemi diversi, dalla rappresentazione di immagini alla definizione di formati di dati.



### Usi

Rispetto all'HTML, l'XML ha uno scopo ben diverso: mentre il primo definisce una grammatica per la descrizione e la formattazione di pagine web (layout) e, in generale, di ipertesti, il secondo è un metalinguaggio utilizzato per creare nuovi linguaggi, atti a descrivere documenti strutturati. Mentre l'HTML ha un insieme ben definito e ristretto di tag, con l'XML è invece possibile definirne di propri a seconda delle esigenze.

L'XML è oggi molto utilizzato anche come mezzo per l'esportazione di dati tra diversi DBMS.



### Sintassi di base

Ecco un esempio tipico di file XML, visualizzabile all'interno di un browser qualsiasi semplicemente salvando il testo in un file con estensione .xml.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<utenti>
    <utente>
        <nome>Luca</nome>
        <cognome>Cicci</cognome>
        <indirizzo>Milano</indirizzo>
    </utente>
    <utente>
        <nome>Max</nome>
        <cognome>Rossi</cognome>
        <indirizzo>Roma</indirizzo>
    </utente>
</utenti>
```





## Principali caratteristiche di XML

Le principali caratteristiche del linguaggio XML possono essere riassunte nei tre seguenti punti:

1. la rappresentazione dei dati è sia *leggibile da un essere umano* sia *leggibile dalla macchina*, il che però, non lo rende ottimale per l'occupazione di memoria e larghezza di banda.
2. I dati assumono la forma di *documenti formali*, che ricordano molto i documenti HTML.
3. I dati includono la definizione dei tipi di se stessi, il che è utile, poichè il ricevente non ha bisogno di sapere in anticipo che tipo di dati sta per ricevere.



## SGML

Lo Standard Generalized Markup Language (SGML), è un metalinguaggio definito come standard ISO (ISO 8879:1986 SGML) avente lo scopo di definire linguaggi da utilizzare per la stesura di testi destinati ad essere trasmessi ed archiviati con strumenti informatici, ossia per la stesura di documenti in forma leggibile da computer (machine readable form).

### Descrizione

Principale funzione di SGML è la stesura di testi chiamati **Document Type Definition (DTD)**, ciascuno dei quali definisce in modo rigoroso la struttura logica che devono avere i documenti di un determinato tipo. Si dice che questi documenti rispetto a SGML costituiscono un *linguaggio obiettivo*, ovvero una applicazione.

SGML è dovuto soprattutto all'opera di Charles Goldfarb e discende dal Generalized Markup Language, linguaggio definito negli anni 1960 presso la IBM, da Goldfarb, Mosher e Lorie.

L'idea centrale di SGML è quella di definire linguaggi di marcatura generica chiamata "**marcatura descrittiva**"; ogni linguaggio obiettivo definisce le caratteristiche strutturali dei documenti che governa.

L'organizzazione di un documento in un linguaggio obiettivo non è primariamente focalizzata sulla sua *resa visiva* (che potrebbe differenziarsi molto con l'uso di diversi dispositivi di visualizzazione: stampante, video, sistema Braille, ecc.), ma piuttosto sui **ruoli logico-semantici** che rivestono le parti nelle quali il documento si articola. Come esempi di questi ruoli vanno segnalati: periodi, paragrafi, capitoli (note, citazioni, tabelle), indici delle parti, indici dei nomi, indici degli autori e delle fonti - aggiunte, allegati, ecc.

Per facilitare la composizione dei documenti retti da SGML sono stati sviluppati programmi come Alml.

### Utilizzo originale

SGML fu inizialmente sviluppato per permettere lo scambio di documenti machine-readable (leggibili da un computer) in progetti governativi, legali e industriali, che devono rimanere leggibili per diverse decadi (un periodo di tempo molto lungo nell'ambito dell'informatica).

Inizialmente usato per pubblicazione di testo e basi di dati, una delle sue maggiori applicazioni fu la seconda edizione dell'Oxford English Dictionary (OED), che era ed è interamente formattato usando un linguaggio SGML.



### Terminologia SGML

- _**Documento SGML**_: è un oggetto di dati che può essere descritto utilizzando un linguaggio di markup generico, prendendo le regole di un generico documento di testo (paragrafi, dati testuali e riferimenti a DTD).
- _**Applicazione SGML**_: è un linguaggio marcatore (*markup*) che segue le specifiche SGML.



## DTD: document type definition

Il Document Type Definition (definizione del tipo di documento) è uno strumento utilizzato dai programmatori il cui scopo è quello di definire le componenti ammesse nella costruzione di un documento XML.

Il termine non è utilizzato soltanto per i documenti XML ma anche per tutti i documenti derivati dall'SGML (di cui peraltro XML vuole essere una semplificazione che ne mantiene la potenza riducendone la complessità) tra cui celeberrimo è l'HTML.

In SGML un DTD è necessario per la validazione del documento. Anche in XML un documento è valido se presenta un DTD ed è possibile validarlo usando il DTD.

Tuttavia XML permette anche documenti ben formati, ovvero documenti che, pur essendo privi diDTD, presentano una struttura sufficientemente regolare e comprensibile da poter essere controllata.

Il DTD si può dichiarare all'interno di uno stesso documento XML (dichiarazione inline).



### Esempio di riferimento allo schema DTD (documento HTML)

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
  <head>
    <title>LOGIN</title>
    <meta http-equiv=content-type content="text/html;
                                           charset=iso-8859-1">
    <meta content="mshtml 6.00.2800.1170" name=generator>
    <link <link
    <link
          href="/images/_site/swas.css" type=text/css rel=stylesheet > href="/images/_site/Show_TableDef.css" type=text/css rel=stylesheet >
    href="/_library/styles.css" rel="stylesheet" title="styles" type="text/css">
  </head>
  <body marginheight=1 align=top border=0 topmargin=1 >
    ...
  </body>
</html>
```



### Relazioni tra SGML, HTML e documenti XML

La seguente figura mostra i gradi di relazione che sussistono tra gli standard che sono stati descritti:

![](immagini/lezione-02/01.png)



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