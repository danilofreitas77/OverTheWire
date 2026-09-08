# Bandit 01 → 02

## 🎯 Objetivo

Encontrar a senha necessária para acessar o próximo nível.

O desafio apresenta um arquivo cujo nome é:

```text
-
```

O objetivo é conseguir visualizar o conteúdo desse arquivo.

## 🛠️ Ferramentas

* Kali Linux
* Terminal
* `ls`
* `cat`

## 🔎 Investigação

Primeiro, listei os arquivos existentes no diretório:

```bash
ls -la
```

Foi identificado um arquivo chamado:

```text
-
```

O problema é que `-` possui um significado especial para muitos comandos Linux.

Por exemplo:

```bash
cat -
```

faz com que o `cat` interprete `-` como **entrada padrão (stdin)**, em vez de tratar `-` como o nome de um arquivo.

## 💡 Solução

Para deixar claro que `-` representa um arquivo localizado no diretório atual, utilizei um caminho relativo:

```bash
cat ./-
```

O conteúdo exibido era a senha necessária para avançar para o próximo nível.

> 🔒 A senha não é armazenada neste repositório para evitar spoilers.

## 🧠 O que aprendi

* Diferença entre argumentos e caminhos de arquivos.
* Conceito de `stdin`.
* Utilização de caminhos relativos.
* Significado de `./` no Linux.
* Como caracteres especiais podem alterar o comportamento de comandos.

## 💡 Principal aprendizado

O desafio parecia extremamente simples, mas mostrou algo importante:

> **Às vezes, o problema não está no comando que você conhece, mas na forma como o sistema interpreta aquilo que você passou para ele.**

Esse foi meu primeiro contato com uma pegadinha típica de CTF.

## ✅ Status

**Concluído**
