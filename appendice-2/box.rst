Box
---

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
                :class: admonition-deepening display-page
      * 
        - Esempio 
        - .. code-block:: rst

             .. admonition:: example
                :class: admonition-example display-page
                
                .. role:: admonition-internal-title
                   :class: admonition-internal-title
             
                `Titolo interno al box`:admonition-internal-title:
      * 
        - RFC 2119: la semantica di questi box è quella espressa nel `Request
          for Comments 2119 <https://www.ietf.org/rfc/rfc2119.txt>`_.
        - .. code-block:: rst
             
             .. admonition:: must
          
          .. code-block:: rst
             
             .. admonition:: should
          
          .. code-block:: rst
             
             .. admonition:: may
          
          .. code-block:: rst
             
             .. admonition:: must-not
          
          .. code-block:: rst
             
             .. admonition:: should-not
      *
        - Usa e non usare
        - .. code-block:: rst
             
             .. admonition:: use
          
          .. code-block:: rst
             
             .. admonition:: use-not
      *
        - Generico con titolo arbitrario
        - .. code-block:: rst
             
             .. admonition:: titolo del box
