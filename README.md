
# Sistema TechOS - Gestão de Ordens de Serviço

## Informações do Projeto

**Instituição:** SENAI Pernambuco  
**Unidade:** Belo Jardim  
**Curso:** Técnico em Desenvolvimento de Sistemas  
**Aluno:** everton emanoel  
**Docente:** Ryan Oliveira  

## Descrição

O TechOS é um sistema de gerenciamento de ordens de serviço desenvolvido para a empresa TechServices.

O sistema permitirá cadastrar clientes, equipamentos e ordens de serviço, além de acompanhar o andamento dos atendimentos.

## Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript
- Node.js
- Express
- PHP
- MySQL
- Git
- GitHub

## Objetivo

Desenvolver uma aplicação web para facilitar o gerenciamento de serviços técnicos.
## Arquitetura do Sistema

O TechOS segue o padrão arquitetural Cliente-Servidor dividido em 3 camadas:

- **Frontend (Apresentação):** Interface web responsiva construída com HTML5, CSS3 e JavaScript, comunicando-se de forma assíncrona via Fetch API.
- **Backend (Aplicação):** API RESTful responsável pelas regras de negócio, validação e autenticação JWT, recebendo e enviando payloads em formato JSON via protocolo HTTP.
- **Banco de Dados (Persistência):** SGBD relacional MySQL (porta 3306) gerenciado via XAMPP e MySQL Workbench.

![Diagrama de Arquitetura TechOS](docs/arquitetura-techos.png)