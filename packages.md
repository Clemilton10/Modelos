# Pacotes

[Modelos](./README.md)

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

[Modelos](./README.md)
