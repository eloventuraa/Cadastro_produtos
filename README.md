# 🛒 Cadastro de Produtos

Projeto desenvolvido para o desafio de cadastro de produtos utilizando HTML, PHP e banco de dados MySQL.

---

## 👤 Autor

* **Aluno(a):** Eloísa Ventura
* **Turma/Sala:** 1ID-DS

---

## 📌 Sobre o Projeto

Este projeto consiste em um sistema simples de cadastro de produtos via formulário web. As informações digitadas pelo usuário são validadas no lado do servidor em PHP antes de serem salvas no banco de dados MySQL.

### ✨ Funcionalidades
* Form visual com campos de **Nome do Produto** e **Preço**.
* Validação de campos obrigatórios (nome não pode estar vazio).
* Validação e conversão de formato numérico para preços (conversão automática de vírgula `,` para ponto `.`).
* Conexão e inserção automática de dados no banco de dados MySQL.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5** — Estruturação do formulário web.
* **PHP** — Processamento dos dados e lógica de validação.
* **MySQL** — Armazenamento persistente dos produtos cadastrados.

---

## 🗄️ Estrutura do Banco de Dados

Para utilizar o projeto, crie o banco de dados `exercicio` e a tabela `produtos` com a seguinte estrutura SQL:

```sql
CREATE DATABASE exercicio;

USE exercicio;

CREATE TABLE produtos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    preco DECIMAL(10, 2) NOT NULL
);
