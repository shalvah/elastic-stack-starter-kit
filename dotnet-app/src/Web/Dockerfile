FROM mcr.microsoft.com/dotnet/core/sdk:2.2 AS build
WORKDIR /app

COPY *.sln .
COPY . .
WORKDIR /app/src/Web

# RUN dotnet restore
ENV ASPNETCORE_ENVIRONMENT Development

EXPOSE 80

ENTRYPOINT ["dotnet", "run"]
