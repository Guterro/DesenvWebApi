# Backend API: Gestão de Produtos com .NET 8 e PostgreSQL

Este repositório contém a aplicação base desenvolvida durante as aulas iniciais da disciplina de **Desenvolvimento de Sistemas Web**, ministrada pelo Professor **Matheus Cataneo** no curso de **Tecnologias da Informação e Comunicação (TIC)** da **UFSC Araranguá**.

## Contexto do Projeto

Este código serviu como o **primeiro contato prático** com a construção de APIs utilizando o ecossistema .NET 8. A estrutura foi fornecida como material de apoio pedagógico para fundamentar os conceitos de:
* Arquitetura de camadas em APIs Web.
* Mapeamento Objeto-Relacional (ORM) com Entity Framework Core.
* Integração e persistência de dados com PostgreSQL.
* Documentação interativa com Swagger.

**Importante:** Esta etapa do projeto é um "checkpoint" de aprendizado e servirá como a base técnica para o desenvolvimento do projeto final da disciplina, onde aplicarei as funcionalidades e lógicas específicas do sistema a ser construído.

---

## Tecnologias Utilizadas

* **Framework:** .NET 8 SDK (C#)
* **ORM:** Entity Framework Core 8
* **Banco de Dados:** PostgreSQL
* **Documentação:** Swagger (OpenAPI)
* **Interface de Gerenciamento:** pgAdmin 4

---

## Estrutura da API (CRUD de Produtos)

A base implementa um fluxo completo de gerenciamento de uma entidade `Produto`:

| Método | Endpoint | Funcionalidade |
| :--- | :--- | :--- |
| **GET** | `/api/produtos` | Lista todos os registros. |
| **GET** | `/api/produtos/{id}` | Busca um registro por ID. |
| **POST** | `/api/produtos` | Insere um novo registro. |
| **PUT** | `/api/produtos/{id}` | Atualiza um registro existente. |
| **DELETE** | `/api/produtos/{id}` | Remove um registro do banco. |

---

## Como Configurar e Rodar

### 1. Requisitos
* [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
* [PostgreSQL](https://www.postgresql.org/download/)
* Instalação da ferramenta EF Core:
  ```bash
  dotnet tool install --global dotnet-ef