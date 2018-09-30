Box
===

Nel corpo dei documenti è possibile inserire i seguenti tipi di box.

.. table:: Tipi di box in Docs Italia
   :name: box-docs-italia

   .. list-table::
      :header-rows: 1

      * 
        - Box
        - Sintassi

      * 
        - Nota
        - .. code-block:: rst
             .. note::
      * 
        - Errore 
        - .. code-block:: rst
             .. error::
      * 
        - Suggerimento 
        - .. code-block:: rst
             .. hint::
      * 
        - Attenzione 
        - .. code-block:: rst
             .. attention::
      * 
        - Importante 
        - .. code-block:: rst
             .. important::
      * 
        - Approfondimento (il box, che può essere espanso, 
          mostra solo una parte del testo 
        - .. code-block:: rst
             .. admonition:: deepening
                :class: admonition-deepening admonition-display-page
             
      * 
        - Esempio 
        - .. code-block:: rst
             .. admonition:: example
                :class: admonition-example admonition-display-page
                
                .. role:: admonition-internal-title
                   :class: admonition-internal-title
             
                `Titolo interno al box`:admonition-internal-title:
                          

