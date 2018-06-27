.. _scrivere-un-documento:

Scrivere un documento
=====================

.. _sec-sintassi:

Il formato reStructuredText (RST)
---------------------------------

I testi di partenza per la pubblicazione su Docs Italia devono essere in `formato reStructuredText <https://it.wikipedia.org/wiki/ReStructuredText>`__ (di seguito anche .rst o RST). Si tratta di file di testo redatti secondo `specifiche regole sintattiche <http://docutils.sourceforge.net/rst.html>`__. La formattazione è ottenuta tramite speciali combinazioni di caratteri, che vengono interpretate da Docs Italia durante la creazione delle pagine.

L’esempio nella :numref:`Tabella %s <cfr-rst>` illustra come è possibile indicare il titolo del documento e una sezione, nonché come ottenere testo in grassetto e in corsivo. Consulta una `guida rapida alla sintassi RST <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`__, oppure la `lista completa delle specifiche del linguaggio <http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html>`__.

.. _cfr-rst:

.. table:: Confronto fra testo RST e testo interpretato.

   +--------------------------------+-----------------------------+
   | **Testo in formato RST**       | **Testo interpretato**      |
   +================================+=============================+
   | .. code-block:: rst            |                             |
   |                                |                             |
   |    ***********************     | **Il titolo del documento** |
   |    Il titolo del documento     |                             |
   |    ***********************     | Lorem ipsum...              |
   |                                |                             |
   |    Lorem ipsum...              |                             |
   |                                |                             |
   |    Una sezione                 | **Una sezione**             |
   |    ==============              |                             |
   |                                | Una frase **in grassetto**. |
   |    Una frase **in grassetto**. |                             |
   |                                | Una frase *in corsivo*.     |
   |    Una frase *in corsivo*.     |                             |
   |                                |                             |
   |                                |                             |
   |                                |                             |
   |                                |                             |
   +--------------------------------+-----------------------------+

Per maggiore chiarezza [in questo repository](https://github.com/italia/docs-italia-esempiformattazione-docs) forniamo un documento di esempio contenente gli elementi di base per la documentazione. Il documento è leggibile in formato RST e nei formati usati da Office e LibreOffice, per un facile confronto.

Strumenti utili
---------------


Editor di testo
~~~~~~~~~~~~~~~

Per la creazione e la modifica dei file RST è sufficiente un editor di testo. In linea di principio, qualsiasi editor può essere usato, anche se alcuni programmi risultano più efficaci di altri. Ecco alcuni suggerimenti.

**Atom**

`Atom <https://atom.io/>`__ è un editor di testo avanzato, open source e sviluppato da GitHub, che permette la creazione e modifica, fra gli altri, di documenti in formato .rst. Atom consente di evidenziare adeguatamente il markup RST.

Questo editor è disponibile per varie piattaforme: Linux, Windows, MacOS.

**Notepad++**

`Notepad++ <https://notepad-plus-plus.org/>`__ è un editor di testo open source disponibile per il sistema operativo Windows. Come Atom, permette la creazione e modifica di documenti in formato .rst con visualizzazione del linguaggio di markup RST.

**Online Editor**

Oltre agli editor stand alone, è disponibile anche il seguente editor online `rst.ninjs.org <http://rst.ninjs.org/>`__ che permette di creare, modificare e visualizzare istantaneamente documenti in formato .rst secondo la logica WYSIWYG (What You See Is What You Get).

**Tabelle .rst**

Per realizzare le tabelle in formato .rst è possibile utilizzare un `editor di tabelle online <http://truben.no/table/>`__.

Convertitore di testi: pandoc
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`pandoc <https://pandoc.org/>`__ è un programma da linea di comando che permette di convertire documenti in formato DOCX e ODT verso diversi `formati di markup <https://it.wikipedia.org/wiki/Linguaggio_di_markup>`__, incluso il formato .rst.

Questo programma permette di migrare su Docs Italia la documentazione prodotta in altri formati, limitando l’intervento manuale. Le operazioni necessarie e i possibili problemi sono descritti nella sezione `Migrazione su Docs Italia di documentazione esistente <#migrazione-su-docs-italia-di-documentazione-esistente>`__.

Per l’installazione del convertitore, puoi fare riferimento alla `pagina ufficiale <https://pandoc.org/installing.html>`__.

Creazione di documenti in formato RST
-------------------------------------

Il primo aspetto rilevante per scrivere una documentazione efficace è `adottare il punto di vista degli utenti che la useranno <https://gdstechnology.blog.gov.uk/2016/10/28/writing-documentation-for-developers/>`__, in questo caso in particolare funzionari e tecnici della Pubblica Amministrazione e dei suoi fornitori. Scrivi il tuo testo seguendo i suggerimenti sulla struttura e sul linguaggio illustrati nella :ref:`guida di stile in appendice <appendice-2>`. Puoi includere nel tuo documento titoli, tabelle, immagini e link esterni, utilizzando la sintassi opportuna.

Il contenuto del tuo testo può essere diviso in vari file .rst per facilitare l’organizzazione e la lettura. Tale divisione può avvenire tipicamente a livello di capitolo o di sezione (vedi anche :ref:`Struttura del repository <sec-struttura>`). Docs Italia combinerà insieme i file per creare l’intero documento, rispettando i link interni e la struttura.


.. note:: 

   File separati diventeranno pagine HTML separate, facilitando la lettura da parte dell’utente.


+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Procedura.**                                                                                                                                                                  |
|                                                                                                                                                                                 |
| -  Scrivi il testo utilizzando il tuo editor preferito o `uno di quelli suggeriti da noi <#editor-di-testo>`__. Utilizza la sintassi RST per titoli, sottotitoli, liste e link. |
|                                                                                                                                                                                 |
| -  Salva il tuo file in formato .rst. In alcuni editor, specie su Windows, potrebbe essere necessario selezionare “Tutti i file” e aggiungere l’estensione manualmente.         |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Migrazione su Docs Italia di documentazione esistente
-----------------------------------------------------

Nel caso in cui si abbiano già dei documenti di partenza (per esempio, in formato DOCX o PDF), questi devono essere convertiti in RST per poter essere pubblicati su Docs Italia. La conversione è in parte automatica ma necessita di una revisione manuale.


Conversione con pandoc
~~~~~~~~~~~~~~~~~~~~~~

Lo strumento di conversione principale verso RST è `pandoc <https://pandoc.org/>`__, uno strumento gratuito open-source.

.. note:: 

   -  pandoc accetta documenti in formato DOCX, ma non in formato DOC.
   
   -  pandoc non accetta documenti in formato PDF.                  


+-----------------------------------------------------------------------------------------+
| **Procedura. Conversione di un documento**                                              |
|                                                                                         |
| -  Se il documento di partenza è un PDF, è necessaria una prima conversione verso DOCX. |
|                                                                                         |
|    -  In Adobe Acrobat, seleziona File -> Export to -> Microsoft Word -> Word Document. |
|                                                                                         |
|    -  Scegli il nome del file e clicca su Save.                                         |
|                                                                                         |
| -  Da linea di comando, esegui:                                                         |
|                                                                                         |
|    :code:`pandoc <percorso/documento> -t rst -o output.rst`                             |
|                                                                                         |
|    dove :code:`<percorso/documento>` è il percorso al documento in formato DOCX.        |
|                                                                                         |
| -  Controlla la conversione automatica ed esegui una revisione manuale del testo        |
+-----------------------------------------------------------------------------------------+

Supporto alla conversione
~~~~~~~~~~~~~~~~~~~~~~~~~

Oltre al processo di conversione illustrato di seguito, Docs Italia mette a disposizione un supporto alla conversione gratuito. L’utente può inviare i documenti da convertire tramite `Slack di Developers Italia <https://slack.developers.italia.it/>`__ usando il canale `#docs-italia <https://developersitalia.slack.com/messages/C9T4ELD4G/>`__. Docs Italia provvederà a rimandare un documento RST corretto e sintatticamente valido. Rimane però responsabilità dell’utente verificare che i contenuti siano corretti.

Revisione dei contenuti e correzione degli errori
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

La revisione del testo è necessaria perché la conversione automatica può presentare degli errori di sintassi. Talvolta, le tabelle costituiscono un elemento problematico, specie quelle con struttura non regolare (ad es., presenza di celle multiple o tabelle annidate).

Per correggere gli errori, è necessaria una **revisione manuale del file** utilizzando uno degli editor di documenti RST già presentati. Alcuni editor consentono di visualizzare un’anteprima automatica delle modifiche al testo (consulta la sezione `Editor di testo <#editor-di-testo>`__). Correggi uno a uno gli errori di formattazione che si presentano, assicurandoti di rispettare la `sintassi dei documenti .rst <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`__.

Eliminati gli errori di sintassi, è necessario uniformare il documento allo `stile di Docs Italia <https://design-italia.readthedocs.io/it/stable/>`__. Consulta la :ref:`Guida di stile contenuta nell’Appendice 2 <appendice-2>` per maggiori informazioni.


