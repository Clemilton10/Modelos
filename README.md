# Modelos

[DotNet](./dotnet.md)

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Solução em branco

```sh
dotnet new sln -n solucao
```

Uma solução pode conter várias aplicações desde aplicativos do console, Aplicações Web, APIs, Bibliotecas, etc.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Aplicativo do console

```sh
dotnet new console -f net6.0 -n consoleName
dotnet sln add consoleName
```

Aplicativo do console(Shell/Tela Preta).

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Aplicativo Web ASP.NET Core

    Home | Privacy

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) ASP.NET Core Vazio

    Hello World!

```sh
dotnet new web -f net6.0 -n webName
dotnet sln add webName
```

    Hello World!

Aplicação Web com apenas a rota padrão `GET` `/` com a mensagem `Hello World!`.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) API Web do ASP.NET Core

![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/swagger.svg)

```sh
dotnet new webapi -f net6.0 -n webapiName
dotnet sln add webapiName
```

Aplicação Web com Controladores `(Controllers)`, com `Swagger` instalado, com a rota padrão `GetWeatherForecast`.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Aplicativo Web do ASP.NET Core (Model-View-Controller)

```sh
dotnet new mvc -f net6.0 -n mvcName
dotnet sln add mvcName
```

<b>M</b>odel-<b>V</b>iew-<b>C</b>ontroller

Aplicação Web com a pasta de modelos `(Models)`, de visualização `(Views)` páginas `Razor`, e dos Controladores `(Controllers)`.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Biblioteca de Classes

```sh
dotnet new classlib -f net6.0 -n biblioteca
dotnet sln add biblioteca
```

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Projeto de Teste do xUnit

```sh
dotnet new xunit -n teste
dotnet sln add teste
```

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

![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) ASP.NET Core Vazio

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

[DotNet](./dotnet.md)
