# Recebi - Sistema de Gestão de Encomendas para Condomínios

O **Recebi** é uma plataforma digital centralizada desenvolvida para modernizar e otimizar a gestão e rastreabilidade de encomendas em condomínios residenciais. O sistema substitui registros manuais por um fluxo digital auditável que monitora desde a entrada do pacote pelo porteiro até a retirada pelo morador.

## 🚀 Funcionalidades Principais

* **Módulo do Porteiro:** Registro de encomendas com descrição, código de rastreio e vínculo automático ao morador/apartamento.
* **Módulo do Morador:** Painel para consulta de encomendas pendentes, retiradas e histórico pessoal.
* **Módulo do Síndico:** Gestão completa de usuários (CRUD) e auditoria global através de logs de segurança.
* **Segurança Jurídica:** Rastreabilidade total garantida por logs automáticos que registram o estado anterior e posterior dos dados (`RegistrarHistoricoAsync`).
* **Controle de Acesso:** Autenticação baseada em tokens (RBAC) com sessões de 8 horas e diferenciação de perfis.

## 🛠️ Tecnologias Utilizadas

* **Backend:** Python com framework Flask
* **Arquitetura:** MVC (Model-View-Controller)
* **Banco de Dados:** MySQL (Relacional)
* **Frontend:** HTML, CSS e JavaScript (com Fetch API para comunicação assíncrona)
* **Comunicação:** API RESTful com dados em formato JSON
* **Autenticação:** Sistema baseado em Tokens JWT

## 📋 Pré-requisitos

Antes de começar, é necessário ter instalado (preferencialmente via WSL/Ubuntu):
* Python 3.10+
* MySQL Server
* Git

## 🔧 Instalação e Configuração

Siga os passos abaixo para configurar o ambiente de desenvolvimento local:

1.  **Clonar o repositório:**
    ```bash
    git clone <url-do-seu-repositorio>
    cd projeto_recebi
    ```

2.  **Criar o ambiente virtual (venv):**
    ```bash
    python3 -m venv venv
    ```

3.  **Ativar o ambiente virtual:**
    ```bash
    source venv/bin/activate
    ```

4.  **Instalar as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

5.  **Configurar as Variáveis de Ambiente:**
    * Crie um arquivo chamado `.env` na raiz do projeto.
    * Copie o conteúdo de `.env.example` e insira as suas credenciais locais do MySQL.

6.  **Preparar o Banco de Dados:**
    * No terminal do MySQL, crie o banco de dados:
    ```sql
    CREATE DATABASE recebi_db;
    ```

7.  **Executar a aplicação:**
    ```bash
    python run.py
    ```
    O servidor estará disponível em `http://127.0.0.1:5000`.

## 👥 Equipe (CC3N - UVV)

* Ana Carollina Silva Dias Ferreira
* Lucas Cunha Missagia
* Pedro Quinellato Dutra Vieira

---
**Data do Projeto:** 25 de abril de 2026
**Instituição:** Universidade Vila Velha (UVV)