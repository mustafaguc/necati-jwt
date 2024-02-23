FROM mcr.microsoft.com/dotnet/sdk
WORKDIR /app
COPY src .
RUN dotnet restore
RUN dotnet publish -o ./publish
ENV ASPNETCORE_URLS=http://+:8001
ENTRYPOINT ["dotnet", "publish/courseservice.dll"]