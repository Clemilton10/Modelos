# Dotnet

```sh
# Listar pacotes
dotnet list package

# instalar pacotes pelo XML
dotnet restore

# Adicionar pacotes
dotnet add package nome

# Remover pacotes
dotnet remove package nome

# Limpar
dotnet clean

# Executar
dotnet run
dotnet run --urls "https://localhost:5000"
dotnet watch run

# Criar o executável
dotnet build

dotnet --version
dotnet --list-sdks
dotnet --list-runtimes

dotnet run
dotnet watch run
dotnet restore
dotnet clean
dotnet build
```

# Modelos

## ![](./vs.svg) Solução em branco

```sh
dotnet new sln -n solucao
```

Uma solução pode conter várias aplicações desde aplicativos do console, Aplicações Web, APIs, Bibliotecas, etc.

## ![](./vs.svg) Aplicativo do console

```sh
dotnet new console -f net6.0 -n consoleName
dotnet sln add consoleName
```

Aplicativo do console(Shell/Tela Preta).

## ![](./vs.svg) ASP.NET Core Vazio

```sh
dotnet new web -f net6.0 -n webName
dotnet sln add webName
```

Aplicação Web com apenas a rota padrão `GET` `/` com a mensagem `Hello World!`.

## ![](./vs.svg) API Web do ASP.NET Core

```sh
dotnet new webapi -f net6.0 -n webapiName
dotnet sln add webapiName
```

Aplicação Web com Controladores `(Controllers)`, com `Swagger` instalado, com a rota padrão `GetWeatherForecast`.

## ![](./vs.svg) Aplicativo Web do ASP.NET Core (Model-View-Controller)

```sh
dotnet new mvc -f net6.0 -n mvcName
dotnet sln add mvcName
```

<b>M</b>odel-<b>V</b>iew-<b>C</b>ontroller

Aplicação Web com a pasta de modelos `(Models)`, de visualização `(Views)` páginas `Razor`, e dos Controladores `(Controllers)`.

# Pacotes

### Listar

```sh
dotnet list package
```

### Instalar

```sh
dotnet add package packageName --version x.x.x
```

### Desinstalar

```sh
dotnet remove package packageName
```

# Ferramentas

### Ajuda

```sh
dotnet tool list -h
```

### Listar

```sh
dotnet tool list -g
dotnet tool list --local
```

### Instalar

```sh
dotnet tool install -g dotnetsay --version 2.0.0
```

# Criar um manifesto

As ferramentas locais são armazenadas no diretório global do NuGet, seja qual for o que você definiu. Há arquivos de correção para cada ferramenta local que apontam para onde as ferramentas estão dentro desse local `$HOME/.dotnet/toolResolverCache`.

Referências a ferramentas locais são adicionadas a um arquivo dotnet-tools.json em um diretório .config no diretório atual. Se um arquivo de manifesto ainda não existir, crie-o usando a opção ou executando o seguinte comando:`--create-manifest-if-needed`

```sh
dotnet new tool-manifest --create-manifest-if-needed
```

# Identity Server

### Criando o projeto

![](./vs.svg) ASP.NET Core Vazio

```sh
dotnet new web -f net6.0 -n is6
dotnet sln add is6
```

### Instalando os templates

```sh
dotnet new install Duende.IdentityServer.Templates
```

### Injetando o Identity Server no projeto

```sh
dotnet new isaspid --force
```
