# Docker

Imagen Base de SQL Server
	docker pull mcr.microsoft.com/mssql/server:2019-CU8-ubuntu-16.04
	docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=@Fiscal2010" -p 1432:1433 --name MySQLServer2019 -d mcr.microsoft.com/mssql/server:2019-CU8-ubuntu-16.04

	docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=@Fiscal2010" -p 1433:1433 --name MySQLServer2017 -d mcr.microsoft.com/mssql/server:2017-latest

	docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=@Fiscal2010" -p 1433:1433 --name MySQLServer2022 --hostname sql1 -d mcr.microsoft.com/mssql/server:2022-latest

	Conectar desde SQL Management
	servidor: localhost   (en caso de tener dos servidores SQL Server, se deja en un puerto distinto y se especifica localhost,1540)
	user: sa
	clave: @Fi*******10 (ojo mayúscula, números y simbolos)
	
Contenido:
	https://learn.microsoft.com/en-us/sql/linux/quickstart-install-connect-docker?view=sql-server-ver16&pivots=cs1-bash
