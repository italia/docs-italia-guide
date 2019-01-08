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
        - :ref:`Approfondimento <box-approfondimento>` (il box, che può essere espanso, 
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

.. _box-approfondimento:

Il box Approfondimento
~~~~~~~~~~~~~~~~~~~~~~

Nel box Approfondimento è possibile decidere quale parte del contenuto è sempre visibile e quale deve essere mostrata soltanto con il pulsante "Mostra tutto". 
È possibile indicare il contenuto nascosto con il parametro `container: more`, come nell'esempio seguente.

Nel caso in cui non venga usato questo parametro, verranno mostrati automaticamente soltanto i primi quattro elementi del contenuto (paragrafi `<p>`, elenchi `<ul>` o altro tipo di tag).

.. code-block:: rst

   .. admonition:: deepening
      :class: admonition-deepening display-page
   
      Paragrafo di testo visibile.
   
      Paragrafo di testo visibile.
   
      .. container: more
   
         Paragrafo di testo nascosto. Può essere mostrato cliccando su "Mostra tutto".
   
         Paragrafo di testo nascosto. Può essere mostrato cliccando su "Mostra tutto".


Questo codice genera il seguente risultato. 

.. admonition:: deepening
   :class: admonition-deepening display-page

   Paragrafo di testo visibile.

   Paragrafo di testo visibile.

   .. container: more

      Paragrafo di testo nascosto. Può essere visibile cliccando su "mostra tutto".

      Paragrafo di testo nascosto. Può essere visibile cliccando su "mostra tutto".
