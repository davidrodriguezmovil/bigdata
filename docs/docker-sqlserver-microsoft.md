# 🧾 Microsoft SQL Server con Ubuntu (docker)

Basado en la imagen oficial: <https://hub.docker.com/_/microsoft-mssql-server>

- Usuario por defecto (admin): sa
- Clave especificada: 1-2-3-a-a-a-a-a-b-b-b-b-b-c-c-c-c
- Puerto al que conectarse de forma exterior: `41433`: Se elige este puerto ya que el habitual `1433` suele estar bloqueado por algunos filtros automáticos.

~~~~
docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Abc12300" -e "MSSQL_PID=Evaluation" -p 41433:1433  --name sqlpreview --hostname sqlpreview -d mcr.microsoft.com/mssql/server:2022-preview-ubuntu-22.04
~~~~
