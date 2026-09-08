##Objetivo

- O objetivo era descobrir a senha que estava em um arquivo chamado --spaces in this filename--

O problema é que o comando cat interpretaria esse novo como argumentos separados. Então, envolvi-os em aspas simples e ele entendeu como um único argumento.

Assim:

cat ./'--spaces in this filename--'
