Appendice 3. Procedure e convenzioni su GitHub
==============================================

.. _sec-procedure-caricamento:

Procedure di caricamento sul repository remoto
----------------------------------------------

Per caricare i file presenti in un repository locale in un repository remoto, sono disponibili due strategie:

1. Upload tramite interfaccia grafica sul sito `github.com <https://github.com/>`__;

2. Upload da repository Git locale tramite i comandi *clone* e *push*.

Il primo metodo è adatto per chi ha poca familiarità con gli strumenti di controllo versione, mentre il secondo consente maggiore flessibilità ed è adatta a utenti mediamente esperti.

Upload tramite interfaccia grafica
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. topic:: Procedura
   :class: procedure
   
   1. Assicurati di avere tutti i file necessari elencati nella sezione precedente
   
   2. Visita la pagina del repository su GitHub
   
   3. Clicca sul pulsante **Upload files**
   
      .. image:: img/upload.png
         :width: 3.74479in
         :height: 0.36363in
   
   4. Clicca su **choose your files** e seleziona tutti i file che intendi caricare
   
   5. Nel riquadro “Commit changes”, specifica un oggetto del commit nel primo box, e opzionalmente un testo di spiegazione, secondo le modalità descritte nella sezione `Messaggi di commit <#messaggi-di-commit>`__ |
   
   6. Clicca sul pulsante **Commit changes**
   
      .. image:: img/commit.png
         :width: 5.14618in
         :height: 3.50521in

Upload da un repository Git locale
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. topic:: Procedura
   :class: procedure
   
   1. Assicurati di avere tutti i file necessari elencati nella sezione precedente
   
   2. Visita la pagina del repository su GitHub
   
   3. Clicca sul pulsante **Clone or download**
   
   4. Clicca sul pulsante **Copy to clipboard** accanto all’URL del repo
   
      .. image:: img/clone.png
         :width: 3.50521in
         :height: 1.52868in
   
   .. role:: procedure-internal-title
      :class: procedure-internal-title

   :procedure-internal-title:`Da linea di comando, esegui`
   
   1. :code:`cd` alla cartella con i file della documentazione

   2. :code:`git clone <URL>`, dove <URL> è l’URL del repo. Puoi ottenerlo
      facendo semplicemente incolla (CTRL + V oppure CMD + V)

   3. :code:`git add *`

   4. :code:`git commit`

   5. All’apertura dell’editor di testo, scrivi il messaggio di commit, secondo
      le modalità descritte nella sezione `Messaggi di commit`_

   6. :code:`git push origin master`


Messaggi di commit
------------------

Ogni volta che si effettua una modifica nel repository, è necessario utilizzare un commit. Questo viene accompagnato da un messaggio che descrive le modifiche apportate.

Il messaggio di commit si compone di due parti:

1. oggetto del commit (obbligatorio)

2. testo di spiegazione del commit (opzionale)

L’\ **oggetto del commit** è sempre obbligatorio e indica in maniera succinta le modifiche apportate al testo o al codice.

-  Indica *cosa* hai fatto, non *come* o *perché*.

-  Usa uno stile diretto e conciso, spiegando con un’unica frase il commit.

-  Elimina gli articoli e le preposizioni, se necessario (se la frase è troppo lunga).

-  Un buon oggetto di commit dovrebbe completare la frase: “Con questo commit, ho…”.

+------------------------------------------+
| **Esempio. Con questo commit, ho …**     |
|                                          |
| -  modificato la funzione,               |
|                                          |
| -  corretto il bug, migliorato lo stile, |
|                                          |
| -  rimosso variabili inutilizzate,       |
|                                          |
| -  aggiunto paragrafo dopo introduzione  |
+------------------------------------------+

Nell’oggetto del commit si dovrebbe indicare il tipo di commit fra i seguenti:

-  Docs: modifiche alla documentazione

-  Stile: formattazione, riformulazione di frasi, ecc

-  Struttura: modifiche alla struttura del testo

-  Refusi: correzione di piccoli refusi

+---------------------------------------------------------+
| **Esempio. Oggetto del commit**                         |
|                                                         |
| -  Stile: diviso frase troppo lunga                     |
|                                                         |
| -  Docs: creato documentazione                          |
|                                                         |
| -  Struttura: aggiunto abstract prima dell’introduzione |
+---------------------------------------------------------+

Il **testo di spiegazione** del commit è opzionale, e può essere usato per fornire ulteriori dettagli riguardo alle modifiche effettuate. Dev’essere separato dall’oggetto del commit da una linea vuota.

Se il commit risolve una o più issue, è obbligatorio indicarne il numero all’interno del testo di spiegazione.

