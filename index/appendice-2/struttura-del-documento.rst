Struttura del documento
=======================

I documenti pubblicati su Docs Italia devono essere suddivisi in file
differenti. Il file :code:`index.rst` contiene il titolo del documento, un breve
riassunto e l’indice dei contenuti. Il resto del documento è diviso in
capitoli (sezioni di primo livello) che corrispondono ad altrettanti
file.



.. admonition:: example          
   :class: admonition-example admonition-display-page          
                                 
   .. role:: admonition-internal-title        
      :class: admonition-internal-title
                                    
   `Esempio di file index.rst`:admonition-internal-title:  

   .. code-block:: rst

      Titolo del documento
      ====================
      
      .. highlights:
      
         Breve testo che riassume il contenuto del documento. Lorem ipsum dolor
         sit amet, consectetur adipiscing elit.
      
      .. toctree::
         :numbered:
      
         titolo-primo-capitolo
         titolo-secondo-capitolo
      

I file che contengono le diverse sezioni di primo livello devono essere
nominati con il titolo del capitolo, sostituendo tutti gli spazi con il
trattino e omettendo le particelle grammaticali.

Poiché la strutturazione del repository impatta sugli URL generati,
tutti i file devono essere collocati nella radice del repository.

Per documenti particolarmente complessi, che rendono necessaria una
ulteriore suddivisione in file, è possibile creare una directory per
ogni sezione (usando il titolo della sezione) e replicare la struttura
di un documento semplice all’interno di ogni directory.

.. admonition:: example          
   :class: admonition-example admonition-display-page          
                                 
   .. role:: admonition-internal-title        
      :class: admonition-internal-title
                                    
   `Esempio di struttura di un documento complesso`:admonition-internal-title:  

   .. code-block::

      ├── index.rst
      
      ├── titolo-primo-capitolo
      
      │ ├── index.rst
      
      │ ├── primo-paragrafo.rst
      
      │ ├── titolo-interessante.rst
      
      │ └── titolo-sezione.rst
      
      ├── titolo-secondo-capitolo
      
      │ ├── index.rst
      
      │ ├── nuova-sezione.rst
      
      │ └── titolo-molto-molto-lungo.rst
      
      └── titolo-terzo-capitolo
      
      ├── index.rst
      
      ├── paragrafo-rivoluzionario.rst
      
      ├── paragrafo-tecnologico.rst
      
      └── paragrafo-tradizionale.rst
