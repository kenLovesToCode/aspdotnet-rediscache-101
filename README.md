<!-- @format -->

# Asp .Net with Redis

```bash
# create webapi app
$ dotnet new webapi -n "CachingWebApi"

# run redis on docker
$ docker run --name test-redis -dp 6379:6379 redis

# run postgre on docker
$ docker run --name test-pgadmin -e POSTGRES_USER=jovanne -e POSTGRES_PASSWORD=Jovanne1 -dp 5432:5432 postgres:latest

# add package
$ dotnet add package Microsoft.EntityFrameworkCore
$ dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL
$ dotnet add package Microsoft.EntityFrameworkCore.Design
$ dotnet add package Microsoft.EntityFrameworkCore.Tools
$ dotnet add package StackExchange.Redis
$ dotnet add package Microsoft.Extensions.Caching.StackExchangeRedis

# create migration
$ dotnet ef migrations add InitialMigration

# migrate
$ dotnet ef database update

# run
$ dotnet run

disable usehttpsredirection at program.cs
# navigate to the given url from terminal and test on
http://localhost:port/swagger/index.html
```
