# CarApp

CarApp é uma aplicação CRUD simples desenvolvida com ASP.NET Core MVC. Este projeto permite criar, ler, atualizar e excluir registros de carros em um banco de dados SQL Server.

## Requisitos

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) (ou [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-editions-express))

## Instalação

1. **Clone o repositório**

   ```bash
    git clone https://github.com/seu-usuario/CarApp.git
    cd CarApp

2. **Restaurar Pacotes NuGet**
```
dotnet restore
```


3. **Configurar a String de Conexão**
Abra o arquivo appsettings.json e ajuste a string de conexão conforme necessário. Exemplo:

```
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=CarAppDb;Trusted_Connection=True;"
}
```

Se estiver usando uma instância diferente ou autenticação SQL, ajuste a string de conexão de acordo.

4. **Aplicar Migrations**

Crie e aplique as migrations para configurar o banco de dados.
```
dotnet ef migrations add InitialCreate
dotnet ef database update
```

## Executando a Aplicação
1.Iniciar a aplicação
```
dotnet run
```

A aplicação estará disponível em http://localhost:5000 (ou a porta configurada).

2. **Acessar a aplicação**

Abra um navegador e vá para http://localhost:5000 para visualizar a aplicação.

## Estrutura do Projeto

Controllers/: Contém os controladores MVC que gerenciam as ações da aplicação.

Models/: Contém os modelos de dados e o contexto do banco de dados.

Views/: Contém as visualizações (páginas Razor) da aplicação.

wwwroot/: Contém arquivos estáticos como CSS, JavaScript e imagens.
appsettings.json: Configurações da aplicação, incluindo a string de conexão do banco de dados.

![Print](https://prnt.sc/axJapV46Jk70)

