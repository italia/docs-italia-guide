Glossario
---------

Il glossario va inserito in unico file che poi è incluso in una `toctree
dedicata <appendice-2.html#indice>`__. Per generare correttamente i riferimenti ai
termini di glossario è obbligatorio usare la direttiva
`glossary <http://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-glossary>`__
di Sphinx e la seguente struttura.

.. admonition:: example
   :class: admonition-example display-page
   
   .. code-block:: rst


      Glossario
      ---------
      
      A
      -
      
      .. glossary::
      
         atermine
            Definizione del termine. Neque porro quisquam est, qui dolorem 
            ipsum quia dolor sit consectetur, adipisci velit, sed quia non 
            incidunt ut labore et dolore magnam aliquam quaerat.
      
            Duis aute irure dolor in reprehenderit in voluptate velit esse 
            cillum dolore eu fugiat nulla pariatur.
      
         antiopam
            Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
            consectetur, adipisci velit, sed quia non numquam eius modi 
            incidunt ut labore et dolore magnam aliquam quaerat.
      
      B
      -
      
      .. glossary::
      
         btimeam
            Neque porro quisquam est, qui dolorem ipsum quia dolor sit
            consectetur, adipisci velit, sed quia non numquam eius modi
            incidunt ut labore et dolore magnam aliquam quaerat.
      



Per inserire nel testo un riferimento ad un termine di glossario è
necessario usare la sintassi: ``:term:`antiopam```. È possibile anche fare
riferimento ad un termine di glossario senza usare esattamente la stessa
parola presente nel glossario. In questo caso la sintassi è:
``:term:`laudem <antiopam>```.
