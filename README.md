# Modelos

[DotNet](./dotnet.md) | [Identity Server](./identity_server.md) | [Pacotes](./packages.md)

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

```console
Home | Privacy
```

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) ASP.NET Core Vazio

```console
Hello World!
```

```sh
dotnet new web -f net6.0 -n webName
dotnet sln add webName
```

```console
Hello World!
```

Aplicação Web com apenas a rota padrão `GET` `/` com a mensagem `Hello World!`.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) API Web do ASP.NET Core

![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/swagger.svg)

```console
Controllers
```

```sh
dotnet new webapi -f net6.0 -n webapiName
dotnet sln add webapiName
```

Aplicação Web com Controladores `(Controllers)`, com `Swagger` instalado, com a rota padrão `GetWeatherForecast`.

## ![](https://raw.githubusercontent.com/Clemilton10/icons/409d6f8e4996b306276f8c31332e2574ce7b019e/vs.svg) Aplicativo Web do ASP.NET Core (Model-View-Controller)

```console
Controllers
```

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

[DotNet](./dotnet.md) | [Identity Server](./identity_server.md) | [Pacotes](./packages.md)
