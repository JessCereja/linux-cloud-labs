# Lab 01 — Preparação de ambiente Linux para Cloud

## 🎯 Objetivo

Preparar um ambiente Linux para estudos e práticas de Cloud Computing, configurando ferramentas essenciais para trabalhar com terminal, Git, GitHub e AWS.

## 💻 Ambiente utilizado

- Lenovo IdeaPad S145
- Linux Mint 22.3 Xfce
- Python 3.12
- Git
- OpenSSH
- Visual Studio Code
- AWS CLI v2

## 🔧 Preparação do ambiente

Durante a preparação foram realizadas:

- atualização dos pacotes do sistema;
- instalação e validação do Git;
- instalação e validação do Python e pip;
- instalação do Visual Studio Code;
- instalação da AWS CLI v2;
- configuração do Git;
- criação de uma chave SSH;
- autenticação do computador no GitHub via SSH.

## 🔐 GitHub via SSH

Para verificar a comunicação SSH com o GitHub foi utilizado o comando `ssh -T git@github.com`.

Após a configuração, a autenticação foi realizada com sucesso.

## ☁️ AWS CLI

A instalação da AWS CLI foi validada com o comando `aws --version`.

A configuração de credenciais AWS não foi realizada neste momento, pois será feita posteriormente em ambiente de estudos/laboratório.

## 🧪 Comandos de validação

Foram utilizados os seguintes comandos para verificar as ferramentas instaladas:

- `python3 --version`
- `pip3 --version`
- `git --version`
- `ssh -V`
- `aws --version`

## 📚 Aprendizados

Neste laboratório pratiquei a preparação de um ambiente Linux, utilização do terminal, configuração inicial do Git e autenticação SSH com o GitHub.

Este ambiente será utilizado nos próximos laboratórios de Linux, redes e Cloud Computing.