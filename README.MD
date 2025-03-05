Documentação do Projeto Megaman API

Visão Geral

O projeto Megaman API é uma API desenvolvida em .NET Core 3.1, utilizando Entity Framework Core para manipulação de dados e outras bibliotecas auxiliares para o desenvolvimento da aplicação.

Tecnologias Utilizadas

A API foi desenvolvida com as seguintes tecnologias:

.NET Core 3.1 - Framework principal da aplicação.

Entity Framework Core 3.1.8 - ORM para manipulação de banco de dados.

SQL Server - Banco de dados utilizado pela aplicação.

Newtonsoft.Json 12.0.2 - Biblioteca para manipulação de JSON.

Dependências

Dependência

Versão

Link

Microsoft.EntityFrameworkCore

3.1.8

Microsoft.EntityFrameworkCore

Microsoft.EntityFrameworkCore.Design

3.1.8

Microsoft.EntityFrameworkCore.Design

Microsoft.EntityFrameworkCore.SqlServer

3.1.8

Microsoft.EntityFrameworkCore.SqlServer

Newtonsoft.Json

12.0.2

Newtonsoft.Json

Estrutura do Projeto

A organização do projeto segue o seguinte formato de diretórios:

.vs
.vscode
bin
Controllers
Database
middlewares
Models
obj
Properties
Services
appsettings.Development.json
appsettings.json
global.json
MegamanApi.csproj
MegamanApi.sln
Program.cs
Startup.cs

Explicação das Pastas

Controllers: Contém os controladores da API.

Database: Contém as configurações do banco de dados.

middlewares: Implementação de middlewares para a API.

Models: Define as entidades do projeto.

Services: Contém a camada de serviços da aplicação.

Properties: Configurações do projeto.

appsettings.json e appsettings.Development.json: Arquivos de configuração da aplicação.

Program.cs: Classe principal que inicializa a API.

Startup.cs: Define os serviços e configurações iniciais da aplicação.

Endpoints da API

A API expõe os seguintes endpoints:

Buscar todos os robôs

Rota: GET /api/v1/robots

Retorno: Lista de robôs cadastrados no sistema.

Buscar robô por ID

Rota: GET /api/v1/robots/{id}

Parâmetros:

id (int) - Identificador do robô.

Retorno:

200 OK: Dados do robô encontrado.

404 Not Found: Nenhum robô encontrado com o ID fornecido.

Criar um novo robô

Rota: POST /api/v1/robots

Retorno: Confirmação de sucesso.

Considerações Finais

Este projeto segue as boas práticas de desenvolvimento em .NET Core, utilizando arquitetura em camadas e padrões de desenvolvimento modernos. Para mais informações sobre cada tecnologia utilizada, consulte os links das dependências na tabela acima.
