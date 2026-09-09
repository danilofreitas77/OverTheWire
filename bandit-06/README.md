# Objetivo

Encontrar a senha que estava em algum lugar do diretório.

Como comando inicial, dei "ls -la" paara ver.

1. Executei o cd .. para subir de diretório
2. Executei o comando "find . -type f -size 33c -user "bandit7" -group "bandit6" para achar. Nenhum arquivo foi encontrado
3. Subi mais uma vez de diretório com o cd ..
4. Executei o comando "find . -type f -size 33c -user 'bandit7' -group 'bandit6' 2>/dev/null" para esconder o erros de permissão
5. Depois disso foi só caminhar até onde estava o arquivo e executar o cat
