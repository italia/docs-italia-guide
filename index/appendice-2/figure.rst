Figure
======

Le immagini dovrebbero essere inserite all’interno di una figura
(includendo quindi almeno una didascalia). Le figure vanno inserite
usando la direttiva RST
`figure <http://docutils.sourceforge.net/docs/ref/rst/directives.html#figure>`__.

Per avere la possibilità di creare `riferimenti <#link-utili>`__ alla
figura nel corpo del testo, è necessario inserire l’opzione :name: con
un nome che può essere richiamato altrove con un semplice :ref:`testo
del riferimento <name della figura>`.

**È obbligatorio inserire nella direttiva l’opzione :alt: contenente il
testo alternativo della figura e una didascalia**. Il testo alternativo
è visualizzato anche nell’indice delle figure: se non viene specificato
il testo alternativo, nell’indice delle figure apparirà la dicitura
“Nessuna descrizione”.

Il testo alternativo dovrebbe essere usato per nominare il file
dell’immagine (trattini al posto degli spazi e omissione delle
particelle grammaticali).

Esempio:

| .. figure:: mappa-modello-strategico.png
| :alt: Mappa del modello strategico

| :name: mappa modello strategico
| Mappa del modello strategico di evoluzione del sistema

informativo della PA

Si può creare un riferimento all’immagine dell’esempio con

Come previsto dalla :ref:`strategia <mappa modello strategico>\` del
piano triennale.
