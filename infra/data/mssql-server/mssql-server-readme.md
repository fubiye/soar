# MSSQL Server Guide

## Install
```
docker pull mcr.microsoft.com/mssql/server:2022-latest

docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=YourStrong@Passw0rd" \
   -p 1433:1433 --name mssql --hostname mssql \
   -v ~/data/mssql:/var/opt/mssql \
   -d mcr.microsoft.com/mssql/server:2022-latest
```
