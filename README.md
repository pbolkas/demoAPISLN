# demoAPISLN

After cloning this project use ```git submodule update --init``` to clone all referenced projects.

This project uses MSSQL server latest docker image.
Use the commands below to create the required MSSQL container.
 - ```sudo docker pull mcr.microsoft.com/mssql/server:2022-latest```
 - ```sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=MySecretD1ff1cultPassw0rd!" -p 1433:1433 --name sql1 --hostname sql1 -d mcr.microsoft.com/mssql/server:2022-latest```

After running the MSSQL container you can *run* the project using

 - ```dotnet run --project DemoAPI```

You can find a swagger document here: 
 - ```http://localhost:5030/swagger/index.html```


You can run the test project using

 - ```dotnet test```
