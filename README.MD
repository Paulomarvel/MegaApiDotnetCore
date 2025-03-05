# Megaman API

![Capacete do robô](https://github.com/Paulomarvel/MegaApiDotnetCore/blob/master/_docs/Astrobot%20avatar.png)

## 📖 Visão Geral
O projeto **Megaman API** é uma API desenvolvida em **.NET Core 3.1**, utilizando **Entity Framework Core** para manipulação de dados e outras bibliotecas auxiliares para o desenvolvimento da aplicação.

![Documento Normativo](https://github.com/Paulomarvel/MegaApiDotnetCore/blob/master/_docs/Megaman_API_Documentacao.pdf)

## 🚀 Tecnologias Utilizadas
| Tecnologia | Descrição |
|------------|-------------|
| **.NET Core 3.1** | Framework principal da aplicação |
| **Entity Framework Core 3.1.8** | ORM para manipulação de banco de dados |
| **SQL Server** | Banco de dados utilizado |
| **Newtonsoft.Json 12.0.2** | Biblioteca para manipulação de JSON |

## 📦 Dependências
| Dependência | Versão | Link |
|--------------|---------|------|
| Microsoft.EntityFrameworkCore | 3.1.8 | [Microsoft.EntityFrameworkCore](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/) |
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [Microsoft.EntityFrameworkCore.Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/) |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [Microsoft.EntityFrameworkCore.SqlServer](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/) |
| Newtonsoft.Json | 12.0.2 | [Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/) |

## 📂 Estrutura do Projeto
A organização do projeto segue a seguinte estrutura de diretórios:
```bash
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
```

### 📁 Explicação das Pastas
| Pasta | Descrição |
|--------|------------|
| **Controllers** | Contém os controladores da API |
| **Database** | Configurações do banco de dados |
| **middlewares** | Implementação de middlewares |
| **Models** | Define as entidades do projeto |
| **Services** | Camada de serviços da aplicação |
| **Properties** | Configurações do projeto |
| **appsettings.json** | Arquivos de configuração |
| **Program.cs** | Classe principal que inicializa a API |
| **Startup.cs** | Define os serviços e configurações iniciais |

## 🌐 Endpoints da API
A API expõe os seguintes endpoints:

### 🔍 **Buscar todos os robôs**
| Método | Rota |
|--------|----------------|
| `GET` | `/api/v1/robots` |
| **Retorno:** | Lista de robôs cadastrados no sistema |

### 🔍 **Buscar robô por ID**
| Método | Rota |
|--------|------------------|
| `GET` | `/api/v1/robots/{id}` |
| **Parâmetros:** | `id` (int) - Identificador do robô |
| **Retorno:** | `200 OK`: Dados do robô encontrado <br> `404 Not Found`: Nenhum robô encontrado |

### ➕ **Criar um novo robô**
| Método | Rota |
|--------|----------------|
| `POST` | `/api/v1/robots` |
| **Retorno:** | Confirmação de sucesso |

![Capacete aberto do robô](https://github.com/Paulomarvel/MegaApiDotnetCore/blob/master/_docs/imagem%20capacete.webp)

## 📝 Considerações Finais
Este projeto segue as boas práticas de desenvolvimento em **.NET Core**, utilizando **arquitetura em camadas** e padrões modernos. Para mais informações sobre cada tecnologia utilizada, consulte os links das dependências na tabela acima.

