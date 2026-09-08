# Bandit 00 → 01

## 🎯 Objetivo

O objetivo deste nível é realizar o primeiro acesso ao servidor do OverTheWire Bandit utilizando **SSH**.

## 🛠️ Ferramentas

* SSH
* Terminal Linux
* Kali Linux

## 🔐 Conexão

O acesso foi realizado através do protocolo SSH:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

Após a conexão, foi necessário utilizar as credenciais fornecidas pelo próprio desafio.

## 🔎 Resolução

Depois de acessar o servidor, o objetivo era encontrar a informação necessária para avançar para o próximo nível.

Primeiro, listei os arquivos disponíveis no diretório atual:

```bash
ls
```

Entre os arquivos encontrados estava:

```text
readme
```

Para visualizar seu conteúdo:

```bash
cat readme
```

O arquivo continha a senha necessária para acessar o próximo nível.

> 🔒 A senha não é armazenada neste repositório para evitar spoilers.

## 🧠 O que aprendi

* O que é SSH na prática.
* Como realizar uma conexão SSH utilizando uma porta específica.
* Como navegar em um ambiente Linux remoto.
* Como listar arquivos utilizando `ls`.
* Como visualizar arquivos utilizando `cat`.
* A importância de ler e interpretar as informações fornecidas pelo sistema.

## 💡 Principal aprendizado

Meu primeiro contato com um CTF mostrou que nem sempre é necessário utilizar ferramentas complexas.

Muitas vezes, **entender o ambiente e saber utilizar corretamente os fundamentos do Linux é o primeiro passo para resolver um problema de segurança.**

## ✅ Status

**Concluído**
