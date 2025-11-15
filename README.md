<div align="center">
  <img src="https://raw.githubusercontent.com/matheusjfsilva/plataforma-SIIF/main/app/static/img/LOGO.png" alt="Logo SIIF" width="150">
  
  <h1 style="border-bottom: none;">Plataforma SIIF</h1>
  
  <p>
    <strong>Sistema de Interação do Instituto Federal (SIIF)</strong>
    <br>
    Uma plataforma web acadêmica para compartilhamento de materiais e central de suporte ao aluno.
  </p>

  <p>
    <img src="https://img.shields.io/badge/Python-3.11%2B-blue?logo=python" alt="Python">
    <img src="https://img.shields.io/badge/Framework-Flask-black?logo=flask" alt="Flask">
    <img src="https://img.shields.io/badge/Database-SQLAlchemy-darkred?logo=sqlite" alt="SQLAlchemy">
    <img src="https://img.shields.io/badge/Frontend-Bootstrap_5-purple?logo=bootstrap" alt="Bootstrap 5">
  </p>
</div>

---

## 📖 Sobre o Projeto

O **SIIF (Sistema de Interação do Instituto Federal)** é uma plataforma web desenvolvida em Python com o framework Flask, destinada a centralizar a vida acadêmica dos alunos do IFRN.

O objetivo é criar um ambiente unificado onde os estudantes possam compartilhar e encontrar materiais de estudo, além de ter um canal direto e seguro para suporte e denúncias, fortalecendo a comunidade do campus.

Este projeto utiliza o padrão *Application Factory* para organização do código, `SQLAlchemy` para gerenciamento do banco de dados SQLite e `Jinja2` com `Bootstrap 5` para o frontend.

## ✨ Funcionalidades Principais

O projeto atualmente está focado em dois grandes módulos:

### 1. 🗂️ Módulo de Materiais (`/materiais`)
Uma central de arquivos onde os alunos podem contribuir e baixar materiais de estudo.

* **Upload de Arquivos:** Envio de materiais (PDF, ZIP, etc.) com título, descrição e categoria.
* **Sistema de Categorias:**
    * Filtragem de materiais por categorias (ex: "História", "Cálculo I", "Projetos").
    * Criação dinâmica de novas categorias diretamente pelo formulário de upload.
* **Pesquisa Inteligente:** Uma barra de busca que usa `thefuzz` para encontrar materiais por títulos ou descrições com "fuzzy matching" (não precisa ser o nome exato).
* **Gerenciamento:** Download direto pelo navegador e exclusão de materiais (função de admin).

### 2. 🎧 Módulo de Suporte (`/suporte`)
Uma página de ajuda centralizada para tirar dúvidas e registrar ocorrências.

* **FAQ Dinâmico:** Uma seção de "Perguntas Frequentes" carregada diretamente do banco de dados.
* **Busca no FAQ:** A barra de pesquisa principal filtra as FAQs em tempo real, exibindo os resultados que correspondem à pergunta ou resposta.
* **Formulário de Denúncia:** Um formulário seguro para o envio de **denúncias anônimas**, que são salvas no banco de dados para revisão da administração.

---

## 🛠️ Tecnologias Utilizadas

* **Backend:**
    * [Python 3](https://www.python.org/)
    * [Flask](https://flask.palletsprojects.com/) (Framework principal)
    * [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/) (ORM para o banco)
    * [Flask-Login](https://flask-login.readthedocs.io/) (Gerenciamento de sessão de usuário)
    * [Werkzeug](https://werkzeug.palletsprojects.com/) (Segurança de arquivos)
    * [TheFuzz](https://github.com/seatgeek/thefuzz) (Para a pesquisa "fuzzy")
* **Banco de Dados:**
    * [SQLite](https://www.sqlite.org/) (Durante o desenvolvimento)
* **Frontend:**
    * [HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
    * [CSS3](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
    * [Bootstrap 5](https://getbootstrap.com/) (Framework CSS)
    * [Jinja2](https://jinja.palletsprojects.com/) (Template Engine)
    * [Bootstrap Icons](https://icons.getbootstrap.com/)

---

## 📂 Divisão do Projeto (Estrutura)

O projeto está organizado usando o padrão **Application Factory**, o que o torna escalável e fácil de manter.
