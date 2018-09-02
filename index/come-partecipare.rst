Come partecipare
================


Prerequisiti
------------

Docs Italia si basa su `GitHub <https://github.com/>`__ come strumento per pubblicare i documenti (e gestirne le versioni).

Per pubblicare un documento, è necessario avere:

1. Un **account utente su GitHub** (obbligatorio);

2. Un’\ **organizzazione su GitHub** (facoltativa).


Account utente su GitHub
~~~~~~~~~~~~~~~~~~~~~~~~

Se fai parte o lavori per un Ente pubblico e vuoi pubblicare i tuoi documenti su Docs Italia, hai bisogno prima di tutto di un account su GitHub. La registrazione è gratuita e può essere completata seguendo le `istruzioni nella pagina ufficiale <https://help.github.com/articles/signing-up-for-a-new-github-account/>`__.

L’account su GitHub consente l’identificazione dell’utente e permette di effettuare tutte le operazioni in maniera sicura e tracciabile.

Organizzazione su GitHub
~~~~~~~~~~~~~~~~~~~~~~~~

L’Ente pubblico può essere associato a un’\ `organizzazione su GitHub <https://github.com/blog/674-introducing-organizations>`__, o può decidere di `crearne una <https://github.com/organizations/new>`__. Un’organizzazione è un insieme di repository gestiti da più utenti GitHub che collaborano a progetti comuni.

L’organizzazione rappresenta una modalità efficiente di raggruppare tutti i progetti digitali di un Ente pubblico. Offre, inoltre, alcuni vantaggi nella gestione dei permessi degli utenti e opzioni di sicurezza e amministrazione avanzate. Anche l’account organizzazione è gratuito e permette un numero illimitato di repository e collaboratori.

La :numref:`Figura %s <developer>` mostra la pagina dell’organizzazione Developers Italia su GitHub. È possibile notare il numero di repository aperti, le persone che collaborano con l’organizzazione e i team.

.. figure:: img/organizzazione.png
   :width: 6.11458in
   :height: 3.41667in
   :alt: Organizzazione GitHub
   :name: developer


**Se il mio Ente non ha un’organizzazione su GitHub...**

Avere un account di organizzazione non è obbligatorio per poter pubblicare i tuoi documenti su Docs Italia, anche se è fortemente consigliato. Agli Enti che non hanno e non possono creare un’organizzazione su GitHub, **Docs Italia mette a disposizione gratuitamente uno spazio su GitHub Italia** dove ospitare i documenti.

Conoscenza di base su Git
~~~~~~~~~~~~~~~~~~~~~~~~~

Docs Italia usa il `version control system <https://it.wikipedia.org/wiki/Controllo_versione>`__ di `Git <https://git-scm.com/>`__, che permette di gestire le diverse versioni di un documento. La pubblicazione su Docs Italia richiede una conoscenza di base di Git e di alcuni termini collegati. Consulta il :ref:`Glossario minimo <sec-glossario>` in Appendice.

.. note::

   Durante l'iniziale fase beta, Docs Italia richiede un account su `Read the Docs <http://readthedocs.org>`__ per poter accedere alle :ref:`funzionalità di backend <sec-backend>`. 


.. _sec-pubblicare:

Come pubblicare un documento
----------------------------

La pubblicazione di un documento su Docs Italia avviene secondo le seguenti fasi:

1. Procedure di autorizzazione iniziale;

2. Inizializzazione dell’account;

3. Caricamento e modifica dei file nel repository di configurazione;

4. Caricamento e modifica dei file nel repository del documento.

I primi due punti (autorizzazione e inizializzazione) sono richiesti soltanto al primo accesso a Docs Italia. Il caricamento e la modifica dei file contenuti nei repository di configurazione e di documento rientrano, invece, in un processo iterativo, che può essere svolto anche in maniera collaborativa.


Procedure di autorizzazione e di inizializzazione
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Le procedure di autorizzazione e di inizializzazione sono **diverse per l’account utente e l’account organizzazione**. In entrambi i casi, però, tali procedure servono a verificare le credenziali dell’utente

**Opzione 1. Account organizzazione**

L’Ente ha un’organizzazione su GitHub e la documentazione viene ospitata presso l’account dell’organizzazione.

1. Un amministratore dell’account organizzazione invia una richiesta di autorizzazione alla pubblicazione su Docs Italia, tramite `Slack di Developers Italia <https://slack.developers.italia.it/>`__ usando il canale `#docs-italia <https://developersitalia.slack.com/messages/C9T4ELD4G/>`__.

2. Gli amministratori di Docs Italia, effettuate le opportune verifiche, autorizzano l’organizzazione alla pubblicazione.

3. Un amministratore dell’account organizzazione crea un apposito repository di configurazione (che serve a creare le pagine progetto e i documenti). :ref:`Maggiori informazioni sul repository di configurazione <sec-repo-config>` sono disponibili nel capitolo dedicato alla pubblicazione. Un esempio di repository di configurazione si trova nello :ref:`Starter kit <sec-starter-kit>` fornito.

4. Un amministratore dell’account organizzazione crea un repository per il documento. Il nome del repository deve rispettare le `convenzioni sui nomi di Docs Italia <#nome-del-repository-del-documento>`__. Successivamente, l’utente può caricare i file secondo le modalità indicate nella sezione `Repository del documento <#repository-del-documento>`__. Un esempio completo di repository del documento è contenuto nello `Starter kit <#starter-kit>`__.

+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Esempio. Processo di autorizzazione per organizzazioni GitHub**                                                                                                          |
|                                                                                                                                                                            |
| Il Ministero dell’Interno vuole pubblicare su Docs Italia un documento chiamato “Modalità di subentro”, relativo al progetto ANPR.                                         |
|                                                                                                                                                                            |
| Il Ministero dell’Interno ha un’organizzazione su GitHub, la cui amministratrice è Giulia Rossi.                                                                           |
|                                                                                                                                                                            |
| Giulia Rossi invia la richiesta di autorizzazione alla pubblicazione su Docs Italia, e la sua richiesta viene approvata.                                                   |
|                                                                                                                                                                            |
| Giulia Rossi crea, quindi, un repository di configurazione presso l’organizzazione GitHub del Ministero dell’Interno.                                                      |
|                                                                                                                                                                            |
| Giulia Rossi crea, infine, un repository del documento presso l’organizzazione GitHub del Ministero dell’Interno, dove inserirà tutti i file relativi alla documentazione. |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

**Opzione 2. Account utente**

L’Ente non ha un’organizzazione su GitHub e la documentazione viene ospitata presso l’account di Docs Italia.

1. L’utente invia una richiesta di autorizzazione alla pubblicazione su Docs Italia, tramite `Slack di Developers Italia <https://slack.developers.italia.it/>`__ usando il canale `#docs-italia <https://developersitalia.slack.com/messages/C9T4ELD4G/>`__.

2. Gli amministratori di Docs Italia, effettuate le opportune verifiche, autorizzano l’utente alla pubblicazione.

3. Il repository di configurazione, necessario a pubblicare le pagine del progetto e i documenti, è già presente nell’account GitHub di Docs Italia. In questo caso, l’inserimento delle informazioni relative al publisher e all’eventuale progetto sono a carico degli amministratori di Docs Italia.

4. Gli amministratori di Docs Italia creano un repository per il documento e concedono all’utente i privilegi di scrittura.


.. note::
   
   Per l’account utente, tale procedura dovrà essere ripetuta per ciascun nuovo documento inserito su Docs Italia. 

+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Esempio. Processo di autorizzazione per utenti GitHub**                                                                                                                                                                                                        |
|                                                                                                                                                                                                                                                                  |
| Mario Bianchi, il Presidente della Commissione Parlamentare XX, vuole pubblicare su Docs Italia un documento chiamato “Relazione sull’Informatica nella Pubblica Amministrazione”.                                                                               |
|                                                                                                                                                                                                                                                                  |
| La Commissione Parlamentare XX non ha un’organizzazione su GitHub, ma Mario Bianchi ha un proprio account utente.                                                                                                                                                |
|                                                                                                                                                                                                                                                                  |
| Mario Bianchi invia la richiesta di autorizzazione alla pubblicazione su Docs Italia, e la sua richiesta viene approvata.                                                                                                                                        |
|                                                                                                                                                                                                                                                                  |
| Gli amministratori di Docs Italia inseriscono nel repository di configurazione presso l’organizzazione GitHub Italia, tutte le informazioni relative alla Commissione Parlamentare XX e alla relativa Relazione.                                                 |
|                                                                                                                                                                                                                                                                  |
| Gli amministratori di Docs Italia creano, infine, un repository del documento presso l’organizzazione GitHub Italia, concedendo i privilegi di scrittura a Mario Bianchi. In questo modo, Mario Bianchi potrà caricare nel repository la propria documentazione. |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Nome del repository del documento
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nel caso sia tua responsabilità creare il :ref:`repository del documento <sec-repo-doc>`, scegli un nome con questo formato: **nomeprogetto-nomedocumento-docs**.

Per esempio, un documento dal titolo “Istruzioni per il cambio di residenza” all’interno del progetto ANPR potrebbe essere ospitato nel repository **anpr-cambioresidenza-docs**.

Il nome deve sempre finire con **-docs** per segnalare che il repository contiene della documentazione.

Passi successivi
~~~~~~~~~~~~~~~~

Dopo aver creato i repository, è possibile caricare i file per generare la documentazione. Le procedure sono descritte nel capitolo :ref:`Pubblicare un documento <pubblicare-un-documento>`.

.. _sec-amministratori:

Amministratori di Docs Italia e assistenza
------------------------------------------

Docs Italia ha dei maintainer con dei privilegi di amministrazione che permettono loro qualsiasi intervento all’interno della piattaforma. Un maintainer di Docs Italia può, per esempio, gestire gli utenti e rimuovere dei documenti già pubblicati.

Tuttavia, nel caso in cui siano chiamati a supportare la creazione di un documento ospitato in un repository di un’organizzazione GitHub, i maintainer devono farsi autorizzare dagli amministratori del repository specifico.

Le attività di pubblicazione utilizzando GitHub e Docs Italia sono a carico dell’organizzazione o dell’utente. In caso di problemi, è possibile chiedere supporto al **servizio assistenza di Docs Italia** tramite `Slack di Developers Italia <https://slack.developers.italia.it/>`__ usando il canale `#docs-italia <https://developersitalia.slack.com/messages/C9T4ELD4G/>`__.


