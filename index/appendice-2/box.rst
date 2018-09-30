Box
===

Nel corpo dei documenti è possibile inserire i seguenti tipi di box:

+-----------------------------------+-----------------------------------+
| **Box**                           | **Sintassi**                      |
+===================================+===================================+
| Nota                              | .. note::                         |
+-----------------------------------+-----------------------------------+
| Errore                            | .. error::                        |
+-----------------------------------+-----------------------------------+
| Suggerimento                      | .. hint::                         |
+-----------------------------------+-----------------------------------+
| Attenzione                        | .. attention::                    |
+-----------------------------------+-----------------------------------+
| Importante                        | .. important::                    |
+-----------------------------------+-----------------------------------+
| Approfondimento (il box, che può  | .. admonition:: deepening         |
| essere espanso, mostra solo una   |                                   |
| parte del testo)                  | :class: admonition-deepening      |
|                                   | admonition-display-page           |
+-----------------------------------+-----------------------------------+
| Esempio                           | .. admonition:: example           |
|                                   |                                   |
|                                   | :class: admonition-example        |
|                                   | admonition-display-page           |
|                                   |                                   |
|                                   | .. role::                         |
|                                   | admonition-internal-title         |
|                                   |                                   |
|                                   | :class: admonition-internal-title |
|                                   |                                   |
|                                   | \`Titolo interno al               |
|                                   | box`:admonition-internal-title:   |
+-----------------------------------+-----------------------------------+
