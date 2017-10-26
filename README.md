# Deploy on Azure

## Deploy via Commandline
````
az group create --name hybrisdemo --location westeurope
az group deployment create --resource-group hybrisdemo --template-uri https://raw.githubusercontent.com/derdanu/sap-hybris/master/azuredeploy.json
````
## Deploy via Azure Portal 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fderdanu%2Fsap-hybris%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>