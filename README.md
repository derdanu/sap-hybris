# Deploy on Azure

## Deploy via Commandline

### Deploy Prod
````
az group create --name hybrisdemoprod --location westeurope
az group deployment create --resource-group hybrisdemoprod --template-uri https://raw.githubusercontent.com/derdanu/sap-hybris/master/azuredeploy.json --parameters @azuredeploy.parameters.json
````

### Deploy Non-Prod
````
az group create --name hybrisdemononprod --location westeurope
az group deployment create --resource-group hybrisdemononprod --template-uri https://raw.githubusercontent.com/derdanu/sap-hybris/master/azuredeploy.json --parameters @azuredeploy.parameters.non-prod.json
````

## Deploy via Azure Portal 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fderdanu%2Fsap-hybris%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>