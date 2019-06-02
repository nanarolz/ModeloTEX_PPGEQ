# ModeloTEX_PPGEQ
Modelo de trabalhos acadêmicos do PPGEQ/UFRN em latex

Necessita do pacote [abntex2](https://github.com/abntex/abntex2) para funcionar

## Alteração em abntex2.cls

Há um warning que não deixa o pdf ser gerado. Localize o arquivo cls da biblioteca abtex2 e altere a seguinte linha:  

>\renewcommand{\appendixtocname}{\uppercase{#2}}

Por

>\renewcommand{\appendixtocname}{\texorpdfstring{\MakeTextUppercase{#2}}{#2}}

O capítulo 3 contêm instruções de construção e formatação dos documentos em latex - pode e deve ser retirado.
