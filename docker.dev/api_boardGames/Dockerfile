FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build

WORKDIR /app/api_boardGames

COPY ./api_boardGames .

RUN dotnet restore "api_boardGames.csproj"

ENTRYPOINT ["dotnet", "watch", "run", "--urls", "http://dotnet:80"]