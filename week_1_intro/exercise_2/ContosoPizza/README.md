Exercise 2 follow the tutorial
https://learn.microsoft.com/en-us/training/modules/build-web-api-aspnet-core/1-introduction


<h2>VsCode plugins to get</h2>

1. C#
2. C# Dev Kit
3. REST Client

<h2>Commands used</h2>

**Check dotnet SDK list** <br>
```bash
dotnet --list-sdks 
```

**Create ASP.Net Core web-api project**
```bash 
dotnet new webapi -controllers -f net8.0
```

**Run the dotnet project**
```bash
dotnet run
```

**Build dotnet project**
```bash
dotnet build
```


<h2>Docker exercise</h2>

```bash
docker build -t exercise2 .
```

```bash
docker run --rm -p 5050:8080 exercise2
```