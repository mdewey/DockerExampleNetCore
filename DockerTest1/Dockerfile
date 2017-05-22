FROM microsoft/aspnetcore-build
WORKDIR /app
COPY . .


RUN dotnet restore
RUN dotnet publish -c Release -o out

EXPOSE 80/tcp
ENTRYPOINT ["dotnet", "out/DockerTest1.dll"]