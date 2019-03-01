Figure
------

Le immagini dovrebbero essere inserite all’interno di una figura
(includendo quindi almeno una didascalia). Le figure vanno inserite
usando la direttiva RST
`figure <http://docutils.sourceforge.net/docs/ref/rst/directives.html#figure>`__.

Per avere la possibilità di creare `riferimenti <link-utili>`__ alla
figura nel corpo del testo, è necessario inserire l’opzione ``:name:`` con
un nome che può essere richiamato altrove con un semplice ``:ref:`testo
del riferimento <name-della-figura>```.

**Per ragioni di accessibilità, è obbligatorio inserire nella direttiva
l’opzione :alt: contenente il testo alternativo della figura.**

Come contenuto della direttiva ``figure`` è opportuno inserire una didascalia.
Essa è visualizzata anche nell’indice delle figure: se non viene specificata una
didascalia, nell’indice delle figure apparirà la dicitura “Nessuna descrizione”.

Il nome del file contenente l'immagine dovrebbe essere facilmente comprensibile
quindi si dovrebbe evitare di usare nomi come ``image_01.png``. Una buona idea
potrebbe essere quella di usare lo stesso testo dell'opzione `name` facendo
attenzione ad usare i trattini al posto degli spazi e omettere le particelle
grammaticali.

.. admonition:: example
   :class: admonition-example display-page
   
   .. code-block:: rst

      .. figure:: mappa-modello-strategico.png
         :name: mappa-modello-strategico
         :alt: La figura mostra la mappa del modello strategico. Essa è formata
               da una pila di componenti corrispondenti ai diversi capitoli del
               piano triennale.

         Mappa del modello strategico di evoluzione del sistema
         informativo della PA
   
Si può creare un riferimento all’immagine dell’esempio con
``Come previsto dalla :ref:`strategia <mappa-modello-strategico>` del piano
triennale.``
