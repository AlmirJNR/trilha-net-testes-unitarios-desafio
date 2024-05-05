FROM mcr.microsoft.com/dotnet/sdk:6.0-alpine3.18 AS build
WORKDIR /src
COPY ["TestesUnitarios.Desafio.Tests/TestesUnitarios.Desafio.Tests.csproj", "TestesUnitarios.Desafio.Tests/"]
COPY ["TestesUnitarios.Desafio.Console/TestesUnitarios.Desafio.Console.csproj", "TestesUnitarios.Desafio.Console/"]
RUN dotnet restore "TestesUnitarios.Desafio.Tests/TestesUnitarios.Desafio.Tests.csproj"
COPY . .
CMD ["dotnet", "test", "/src/TestesUnitarios.Desafio.Tests", "--no-restore"]