# Azure - Linux Docker Developer Virtual Machine

Azure ARM template that creates Azure Linux VM with following software installed:

* Ubuntu Server 16.04 LTS
* Docker (includes docker engine, client and docker compose)
* Git
* Nodejs
* Dotnetcore 
* Azure Cli
* Yeoman
* Bower

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fubuntu-1604LTS-docker.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fubuntu-1604LTS-docker.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>


After the virtual machine is created and running use the following command to find out versions of all of the installed software:

```
echo 'nodejs version ' $(node -v)  && echo 'npm version ' $(npm -v)  &&  echo 'dotnet version ' $(dotnet --version) && $(git --version) && az --version && printf "docker Client & Server version \n $(docker version)" 
```

# Azure - Windows Container Developer Virtual Machine

Azure ARM template that creates Azure Windows Server 2016 VM with following software installed:

* Windows Server 2016
* Windows Containers - Docker Engine and Docker Compose (NOTE: This template does not support Docker Linux containers running on Windows Server 2016. If you need both Docker Linux containers and Windows Containers use the ARM template below that install Docker for Windows - it does require nested virtualization)
* Chocolatey
* Putty
* Node 
* Dotnetcore
* Azure Cli
* Sql Server Management Studio (SMSS) 17
* Visual Studio Code
* Visual Studio 2017 Community Edition
  
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fwinsrv2016-docker.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fwinsrv2016-docker.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

# Azure - Windows Container Developer Virtual Machine (with Docker for Windows)

Azure ARM template that creates Azure Windows Server 2016 VM with following software installed. Please 
note that Docker for Windows require nested virtualization. That is the reason behind using Standard_D2s_v3 
for this ARM template. 

* Windows Server 2016
* Docker for Windows - Docker Engine and Docker Compose (NOTE: This supports both Docker Linux containers and Windows containers. If you are looking for Windows containers only then use the ARM template above)
* Chocolatey
* Putty
* Node 
* Dotnetcore
* Azure Cli
* Sql Server Management Studio (SMSS) 17
* Visual Studio Code
* Visual Studio 2017 Community Edition
  
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fwin2016-vs2017-docker.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Frazi-rais%2Fmicroservices%2Fmaster%2Freference-material%2Farm-templates%2Fwin2016-vs2017-docker.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>
