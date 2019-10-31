Indice
------

L’indice del documento va inserito nel file index.rst per mezzo della
direttiva di Sphinx
`toctree <http://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree>`__.
Per generare la numerazione delle `sezioni <sezioni.html>`__, delle
`tabelle <tabelle.html>`__ e delle `figure <figure.html>`__, è
necessario usare l’opzione ``:numbered:``. Il contenuto della direttiva è
costituito da un elenco di tutti i file da includere. I file
corrispondono alle sezioni di primo livello.

Il glossario, se presente, non va inserito nella toctree insieme ai file
delle sezioni, ma in una toctree dedicata che non deve avere l’opzione
``:numbered:`` (perché il glossario non va numerato) e deve invece riportare
le opzioni ``:hidden:`` e ``:name: glossary_toc``. Queste opzioni sono
necessarie per fare in modo che Sphinx identifichi e gestisca
correttamente la sezione glossario.


.. admonition:: example
   :class: admonition-example display-page
   
   .. role:: admonition-internal-title
      :class: admonition-internal-title

   `Esempio di toctree con glossario`:admonition-internal-title:

   .. code-block:: rst

      .. toctree::
         :numbered:
      
         titolo-primo-capitolo
         titolo-secondo-capitolo
      
      .. toctree::
         :name: glossary_toc
         :hidden:
      
         glossario
