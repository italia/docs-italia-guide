.. _appendice-2:

Appendice 2. Guida di stile
===========================

Questa appendice fornisce alcune indicazioni sull’organizzazione dei contenuti e lo stile dei documenti su Docs Italia e integra le indicazioni fornite nelle `Linee guida di design per i servizi web della PA <https://design-italia.readthedocs.io>`__.


Organizzazione dei contenuti
----------------------------

**Il tuo testo verrà letto principalmente online.**

Inserisci le informazioni più importanti all’inizio del testo, in modo da fornire subito a chi legge le informazioni che cerca. Utilizza i paragrafi successivi per ulteriori spiegazioni.

Usa il grassetto o il corsivo per mettere in evidenza i punti più importanti e attirare l’attenzione.

**Usa una struttura modulare.**

Una struttura ben definita aiuta a comprendere meglio il testo. Separa le varie sezioni in paragrafi con un titolo rilevante. A volte, un’immagine o una tabella possono fornire più informazioni di un testo.

Nell’organizzare i contenuti, utilizza la seguente struttura modulare:

-  Acronimi

-  Contenuti

-  Domande frequenti (FAQ)

Gli acronimi, se presenti, dovrebbero essere inseriti in testa alla documentazione. Si sconsiglia, nei documenti web, l’utilizzo di lunghe introduzioni: i lettori sono interessati direttamente ai contenuti.

Prima di creare una sezione di FAQ, chiediti se serve davvero [1]_: stai semplicemente duplicando le informazioni? Puoi inserire gli stessi contenuti all’interno della documentazione? Nel caso in cui sia comunque necessario creare una sezione di FAQ, le domande devono essere efficaci, sintetiche e dirette verso il fruitore della documentazione.

**Tipi di contenuti**

Per aiutarti a strutturare meglio il tuo testo, puoi **pensare alla funzione di ciascuna parte** secondo questa tabella (tipica della `documentazione DITA <https://en.wikipedia.org/wiki/Darwin_Information_Typing_Architecture#Information_typing>`__):

+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Concetti               | Descrizioni e spiegazioni relative a un argomento.                                                                                                                                          |
|                        |                                                                                                                                                                                             |
|                        | Formato: paragrafi di testo.                                                                                                                                                                |
|                        |                                                                                                                                                                                             |
|                        | Esempio: `Introduzione a pagoPA <https://pagopa-doc-overview.readthedocs.io/it/latest/introduzione.html>`__                                                                                 |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Procedure              | Lista di operazioni o di passi per ottenere un risultato.                                                                                                                                   |
|                        |                                                                                                                                                                                             |
|                        | Formato: elenco puntato o numerato.                                                                                                                                                         |
|                        |                                                                                                                                                                                             |
|                        | Esempio: `18app, Istruzioni per la compilazione di una fattura <http://guida-18app.readthedocs.io/it/latest/linee-guida-fatturazione.html#istruzioni-per-la-compilazione-di-una-fattura>`__ |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Liste di consultazione | Coppie di indice-valore (per esempio un glossario, lista di funzioni API, ecc).                                                                                                             |
|                        |                                                                                                                                                                                             |
|                        | Formato: tabella a due colonne.                                                                                                                                                             |
|                        |                                                                                                                                                                                             |
|                        | Esempio: `ANPR, Tabella 14. Lingue <https://anpr.readthedocs.io/en/latest/tab/tab_lingue.html>`__                                                                                           |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Frammenti              | Brevi frasi che fungono da connessione fra le varie parti della guida.                                                                                                                      |
|                        |                                                                                                                                                                                             |
|                        | Esempio: “Maggiori informazioni possono essere trovate su questo sito”.                                                                                                                     |
+------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Stile e linguaggio
------------------

Relativamente allo stile da utilizzare, è possibile far riferimento alle `Linee Guida di Design <https://design-italia.readthedocs.io/it/stable/doc/content-design/linguaggio.html#>`__, applicando qualche ulteriore accorgimento dettagliato di seguito.

Caratteri speciali
~~~~~~~~~~~~~~~~~~

Alcuni caratteri speciali possono essere interpretati in maniera errata in fase di compilazione del documento. Per esempio, gli apici obliqui sono utilizzati per definire alcune direttive nel linguaggio RST.

Per questo motivo, utilizza doppi apici dritti invece che doppi apici obliqui, sia in apertura che in chiusura. L’apice obliquo va sostituito con l’apice dritto.

+------------------------------------+---------------------------------+
| **Da evitare**                     | **Consigliato**                 |
+====================================+=================================+
| Doppi apici obliqui: :code:`“ ”`   | Doppi apici dritti: :code:`"`   |
+------------------------------------+---------------------------------+
| Apice obliquo singolo: :code:`‘ ’` | Apice dritto singolo: :code:`'` |
+------------------------------------+---------------------------------+

Codice
~~~~~~

Il codice deve essere visualizzato con carattere *monospace*. Per poter visualizzare il codice con tale formattazione, indipendentemente dal template, è necessario usare il ruolo :code: inserendo il codice tra due apici obliqui.

+-------------------------------------------------------------------+
| **Esempio. Formattazione del codice**                             |
|                                                                   |
| .. code-block:: rst                                               |
|                                                                   |
|    :code:`<aux digit (1n)>[<application code> (2n)]<codice IUV>\` |
|                                                                   |
| **Esempio. Codice reso nel testo**                                |
|                                                                   |
| :code:`<aux digit (1n)>[<application code> (2n)]<codice IUV>`     |
+-------------------------------------------------------------------+

Note
~~~~

L’utilizzo delle note nei documenti web è sconsigliato: a volte, le note possono essere sostituite da `riferimenti <#riferimenti>`__ nel testo (vedi sotto). Se indispensabili, le note devono essere tutte in fondo alla pagina e non, ad esempio, dopo una tabella o alla fine di un paragrafo.

Le note hanno una numerazione indipendente in ciascuna pagina. Per un esempio, consulta il `Piano Triennale per l’Informatica nella PA 2017-2019 <https://pianotriennale-ict.readthedocs.io/it/latest/doc/01_piano-triennale-per-informatica-nella-pa.html>`__.

Riferimenti
~~~~~~~~~~~

All’interno del documento, i riferimenti ad altre parti di testo devono essere corredati da opportuni link.

Quando crei un collegamento a un sito esterno, evita di associare il link a frasi come “clicca qui” oppure “a questo link”. Usa, invece, frasi che descrivono il contenuto del collegamento, come “visita la pagina di aiuto” oppure “consulta la sintassi RST”.

Tabelle
~~~~~~~

Nelle tabelle, il testo di ogni cella inizia sempre con la lettera maiuscola, salvo il caso in cui si faccia riferimento a identificatori che inizino con la lettera minuscola. A fine riga in ciascuna tabella non serve il punto. L’intestazione delle colonne e delle righe di una tabella è in grassetto.

La tabella deve essere preceduta da una didascalia centrata che ne descriva il contenuto.

Le tabelle devono essere numerate in maniera progressiva. Per la numerazione, si può utilizzare l'auto numerazione già presente nel template di Docs Italia. La numerazione manuale è fortemente sconsigliata in quanto introduce un elemento di possibile incoerenza nel documento che si sta scrivendo o che si modificherà in futuro.

.. table:: Esempio di tabella in Docs Italia.

   +-------------------------+-------------------------+-------------------------+-------------------------+
   |                         | **Intestazione col. 1** | **Intestazione col. 2** | **Intestazione col. 3** |
   +=========================+=========================+=========================+=========================+
   | **Intestazione riga 1** | Testo                   | Testo                   | Testo                   |
   +-------------------------+-------------------------+-------------------------+-------------------------+
   | **Intestazione riga 2** | Testo                   | Testo                   | Testo                   |
   +-------------------------+-------------------------+-------------------------+-------------------------+

Figure e immagini
~~~~~~~~~~~~~~~~~

Tutte le figure e le immagini devono essere seguite da opportune didascalie, numerate in maniera progressiva. Per la numerazione delle figure si può utilizzare l'auto numerazione già presente nel template di Docs Italia. La numerazione manuale è fortemente sconsigliata in quanto introduce un elemento di possibile incoerenza nel documento che si sta scrivendo o che si modificherà in futuro.
                                                        
+----------------------------------------------------------+
| **Esempio di figure / immagini in Docs Italia**          |
|                                                          |
| .. figure:: img/logo.png                                 |
|    :width: 6.11458in                                     |
|    :height: 1.31944in                                    |
|    :alt: Esempio di immagine                             |
|    :name: logo                                           |
|                                                          |
|    Logo del Team per la Trasformazione Digitale.         |
+----------------------------------------------------------+

Titoli
~~~~~~

Come già indicato nelle `Linee Guida di Design <https://design-italia.readthedocs.io/it/stable/doc/content-design/linguaggio.html#titoli>`__, nei titoli non dovrebbero essere presenti trattini o slash (-, /, \|).

Nel caso sia necessario utilizzare un segno divisorio, questo dovrebbe essere il punto.

+----------------------------------------+
| **Esempio. Formato del titolo**        |
|                                        |
| Appendice 1. Codici dei regimi fiscali |
+----------------------------------------+

Ottimizzazione SEO
~~~~~~~~~~~~~~~~~~

L’ottimizzazione per i motori di ricerca (in inglese, *search engine optimization* o SEO) è un aspetto importante da tenere presente nella scrittura di un documento. L’obiettivo dell’ottimizzazione SEO dei contenuti è di migliorare il posizionamento del documento fra i risultati delle ricerche degli utenti in corrispondenza di alcune parole chiave. I primi risultati, infatti, sono quelli che ricevono più click e quindi più visite.

Per maggiori informazioni sull’ottimizzazione SEO, puoi consultare il `capitolo dedicato nelle Linee guida di design per i servizi web della PA <https://design-italia.readthedocs.io/it/stable/doc/content-design/seo.html>`__, dove vengono illustrate una serie di tecniche e strategie per migliorare i contenuti dei documenti.

.. [1]
   GOV.UK, nelle proprie linee guida, sconsiglia l’uso delle FAQ: https://www.gov.uk/guidance/content-design/writing-for-gov-uk#dont-use-faqs


.. |image12| image:: img/logo.png
   :width: 6.11458in
   :height: 1.31944in

