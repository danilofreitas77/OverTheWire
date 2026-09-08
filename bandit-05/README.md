# Objetivo:

Achar a senha em um arquivo com tamanho específico, não-executável e com dados legíveis.

Comecei acessando o diretório "inhere", li as pastas que estava lá e fiz um filtro "find . f -size 1033c". Ou seja, um comando que procura no diretório atual arquivos com o tamanho de 1033 bytes.

Depois disso verifiquei as permissões (ls -l) do arquivo encontrado (para ver se era não-executável) e dei o file .(nome do arquivo) para ver o tipo dele.
Depois de verificadas as condições, acessei o arquivo e peguei a password.
