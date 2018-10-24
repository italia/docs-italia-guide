Tabelle
-------

Le tabelle vanno inserite mediante la direttiva RST
`table <http://docutils.sourceforge.net/docs/ref/rst/directives.html#table>`__.

È obbligatorio inserire l’opzione ``:name:`` per avere la possibilità di
creare `riferimenti <appendice-2.html#link-utili>`__ alla tabella nel corpo del testo. 

È obbligatorio inserire una didascalia. La didascalia è visualizzata anche
nell’indice delle tabelle.

Sono disponibili alcune classi (da inserire nell’opzione class) per
stilizzare la tabella.

.. admonition:: example
   :class: admonition-example display-page
   
   .. code-block:: rst

      .. table:: Didascalia testo tabella. Enim ad minim veniam neste.
         :name: attivita-previste
      
         +-----------+-----------+-----------+
         | Lorem     | Vivamus   | Phasellus |
         | ipsum sit | elementum | viverra   |
         | dolor est | semper    | nulla ut  |
         | quantu    | nisi      | metus     |
         | ieres     | aenean    | arius     |
         | numer     | vusere    | laoreet   |
         |           |           | quisque   |
         |           |           | rutrum    |
         +-----------+-----------+-----------+
         | Maecenas  | Cursus    | Fusce     |
         | nec odio  | nunc,     | vulputate |
         | et ante   | quis      | eleifend  |
         | tincidunt | gravida   | sapie ves |
         | tempus    | magna mi  | tibulum   |
         |           | a libero  | purus     |
         |           |           | quam      |
         +-----------+-----------+-----------+
      


