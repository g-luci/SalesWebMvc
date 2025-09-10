# SalesWebMvc

Este é um projeto de aplicação web MVC desenvolvido em ASP.NET Core, que simula um sistema de gestão de vendas. O projeto foi construído como parte do curso "C# COMPLETO Programação Orientada a Objetos + Projetos".

## Descrição do Projeto
A aplicação SalesWebMvc é um sistema web para gerenciar vendedores, departamentos e registros de vendas. O projeto utiliza o padrão de arquitetura MVC (Model-View-Controller) para separar as responsabilidades e garantir uma estrutura organizada.

## Funcionalidades
O sistema oferece as seguintes funcionalidades principais:

* **Vendedores (Sellers):**

    * Listagem de todos os vendedores.

    * Adicionar um novo vendedor.

    * Excluir um vendedor.

    * Visualizar detalhes de um vendedor.

    * Editar as informações de um vendedor.

* **Departamentos (Departments):**

    * Listagem de todos os departamentos.

    * Adicionar um novo departamento.

    * Excluir um departamento.

    * Visualizar detalhes de um departamento.

    * Editar as informações de um departamento.

* **Registros de Vendas (SalesRecords):**

    * Pesquisa simples de vendas por data.

    * Pesquisa agrupada de vendas por vendedor e data.

## Tecnologias Utilizadas
O projeto foi desenvolvido com as seguintes tecnologias e pacotes:

* Linguagem: C#

* Framework: ASP.NET Core MVC (net7.0).

* ORM: Entity Framework Core.

* Banco de Dados: MySQL com o provider Pomelo.EntityFrameworkCore.MySql.

* Frontend: ASP.Net core Razor pages

## Como Executar o Projeto
Para executar a aplicação, siga os passos abaixo:

1. **Clonar o Repositório: Clone este repositório para sua máquina local.**
    ```bash
    git clone https://github.com/g-luci/saleswebmvc.git
    ```

2. **Configurar o Banco de Dados:** O projeto utiliza MySQL. Você precisa ter um servidor MySQL instalado e em execução.

3. **Configurar a Conexão:** Abra o arquivo `appsettings.json` e configure a sua string de conexão com o banco de dados. A chave da conexão é `"SalesWebMvcContext"`.
    ```json
    "SalesWebMvcContext": "server=myServerAddress;userid=myUsername;password=myPassword;database=saleswebmvcappdb"
    ```
4. **Executar Migrações:** Execute o comando do Entity Framework Core para aplicar as migrações:
    ```bash
    dotnet ef database update
    ```

5. **Executar a Aplicação:** Para rodar o projeto, use o comando:
    ```bash
    dotnet run
    ```

