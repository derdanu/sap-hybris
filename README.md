az group  create --name hybrisdemo --location westeurope
az group deployment create --resource-group hybrisdemo --template-file .\azuredeploy.json

az group deployment create --resource-group hybrisdemo --template-uri https://raw.githubusercontent.com/derdanu/sap-hybris
/master/azuredeploy.json

az group delete --name hybrisdemo --location westeurope