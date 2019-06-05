# ModeloTEX_PPGEQ
Modelo de trabalhos acadêmicos do PPGEQ/UFRN em latex.

## Instalando [abntex2](https://github.com/abntex/abntex2ex2

Para instalar o pacote é necessário um programa que o gerencie. O [miktex](https://miktex.org/) funciona para qualquer sistema operacional. Ao instala-lo procure por abntex2 em 'package' e instale.

## Alteração em abntex2.cls (caso necessário)

Há um warning que não deixa o pdf ser gerado. Localize o arquivo cls da biblioteca abtex2 e altere a seguinte linha:  

>\renewcommand{\appendixtocname}{\uppercase{#2}}

Por

>\renewcommand{\appendixtocname}{\texorpdfstring{\MakeTextUppercase{#2}}{#2}}

## Observações

O capítulo 3 contêm instruções de construção e formatação dos documentos em latex - pode e deve ser retirado.
