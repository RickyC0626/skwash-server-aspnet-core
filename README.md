# Skwash Server
Written in ASP.NET Core

## Prerequisites
- [.NET SDK 6.0](https://dotnet.microsoft.com/en-us/download)

## Run Server
In Visual Studio:
- No debugger - `Ctrl + F5`
- With debugger - `F5`

In command line:
```sh
dotnet run
```

## Build Server
```sh
dotnet build
```

## Test API
Feel free to use [Postman](https://www.postman.com), [Insomnia](https://insomnia.rest), or the following CLI tool to test the API.

### HTTP CLI Tool
Install the .NET HTTP REPL command-line tool:
```sh
dotnet tool install -g Microsoft.dotnet-httprepl
```

Connect to the API with the valid port number:
```sh
httprepl http://localhost:5221
```

Alternatively, you can connect to web API while `HttpRepl` is running:
```sh
(Disconnected)> connect http://localhost:5221
```

Explore available endpoints while in `HttpRepl`:
```sh
http://localhost:5221/> ls
.      []
api    []
```

Use `cd` to a specific endpoint:
```sh
http://localhost:5221/> cd api
/api    []
```

```sh
http://localhost:5221/api> ls
.           []
..          []
TodoItems   [GET|POST]
```

#### End Session
```sh
http://localhost:5221/api> exit
```
