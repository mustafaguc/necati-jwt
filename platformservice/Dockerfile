FROM mcr.microsoft.com/dotnet/sdk
WORKDIR /app
COPY src .
RUN dotnet restore
RUN dotnet publish -o ./publish
ENV ASPNETCORE_URLS=http://+:8000
ENTRYPOINT ["dotnet", "publish/platformservice.dll"]