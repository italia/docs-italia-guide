.. _appendice-1:

Appendice 1. Il versionamento
=============================

Introduzione
------------

Il `version control <https://it.wikipedia.org/wiki/Controllo_versione>`__ o versionamento consente di tracciare i cambiamenti occorsi a un file o a un insieme di file. Permette, tra le altre cose, di riportare i file o l’intero progetto a uno stadio precedente, visualizzare le modifiche nel corso del tempo, sviluppare più linee di lavoro in parallelo e identificare gli autori delle modifiche.

I sistemi di controllo versione sono usati abitualmente nei progetti di sviluppo software. Questi sistemi possono essere applicati anche alla documentazione: con un approccio di tipo “\ `docs as code <https://gdstechnology.blog.gov.uk/2017/08/25/why-we-use-a-docs-as-code-approach-for-technical-documentation/>`__\ ” (documentazione come codice), è possibile tracciare i cambiamenti puntuali dei vari file e definire delle versioni.

.. _sec-glossario:

Glossario minimo
----------------

**repository**

Il repository è una cartella in cui vengono conservati tutti i file di un progetto. Questa cartella può essere salvata localmente o ospitata su una piattaforma online come `GitHub <https://github.com/>`__ (repository remoto).

**commit**

Un commit è una *fotografia* del progetto e di tutti i file in un determinato istante. Eseguire un commit significa essenzialmente congelare lo stato del progetto per poterlo recuperare in futuro.

**tag**

Il tag è un’etichetta che punta a uno specifico commit. Può essere usato per identificare degli stadi particolari nell’evoluzione del progetto (ad es. le *release*, ovvero i rilasci del software o della documentazione).

Tipi di versionamento
---------------------

Docs Italia utilizza il sistema di controllo versione di GitHub: per ogni documento, esiste una traccia pubblica di tutte le modifiche effettuate e dei relativi autori.

Il versionamento adotta un **sistema di release basato sui tag**, che varia in base al tipo di documento.

**Documentazione di un progetto software**

Il versionamento del codice e della relativa documentazione vanno di pari passo.

Dal momento che non è possibile imporre una singola strategia di versionamento, le versioni della documentazione avranno formati diversi a seconda del tipo di versionamento usato per il software.

**Linee guida**

La versione viene indicata dall’anno e da un numero progressivo, nel formato **AAAA.N**. Ad esempio, la versione numero 1 dell’anno 2018 sarà indicata con 2018.1. È possibile `estendere il processo di versionamento <#estensione-del-processo-di-versionamento>`__ alle fasi di consultazione e approvazione.

**Testo legislativo**

La versione del documento è determinata dalle modifiche introdotte nel corso dell’iter legislativo.

La versione viene indicata dalla data in cui è approvata una modifica al testo, nel formato **vAAAA-MM-GG**. Ad esempio, un testo modificato tramite Decreto Legislativo del 13 dicembre 2017 sarà associato alla versione v2017-12-13.

Vedi il `Codice dell’amministrazione digitale <http://cad.readthedocs.io>`__ per un esempio.

Estensione del processo di versionamento
----------------------------------------

Per tenere conto di alcune esigenze relative al procedimento amministrativo, è possibile estendere il versionamento del documento descritto sopra. In particolare, per ciascun documento sono previste diverse fasi di sviluppo.

**Documento in fase di creazione**

Il documento non è ancora pubblico. Su Docs Italia esiste solo il titolo, con l’etichetta “Documento in fase di creazione”. Il documento può essere contenuto in un repository pubblico o privato di GitHub. La stesura si potrebbe iniziare già su GitHub, che supporta perfettamente un approccio collaborativo.

**Documento in bozza (versione alfa, con tag)**

Il documento è pubblicato come bozza, in consultazione. I nuovi contenuti e le modifiche ai contenuti esistenti, dopo essere approvati, vengono pubblicati nella versione alfa del documento. Vengono resi disponibili per una discussione pubblica e una revisione da parte della community, anche se questa è priva di valore ufficiale.

**Documento firmato, in attesa di parere (versione beta, con tag)**

Il documento è firmato, in attesa di parere positivo. In Docs Italia sarà presente, oltre al PDF del documento, anche il PDF firmato relativo allo stesso documento in pubblicazione.


**Documento approvato (release, con tag)**

Il documento ha ricevuto parere positivo e viene pubblicato in via ufficiale. Su Docs Italia appare anche come **versione stable**.

**Successive modificazioni (versione latest)**

Le modifiche intermedie apportate al documento, quando non esplicitamente associate a una versione come descritto sopra, vengono indicate con la generica versione **latest**. In questo caso vengono visualizzate le modifiche più recenti, senza però che il documento abbia valore ufficiale.

.. figure:: img/versionamento.png
   :width: 5.14583in
   :height: 4.53172in
   :alt: flusso di versionamento
   :name: versionamento
   
   Esempio di flusso di versionamento.
