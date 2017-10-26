az group  create --name hybrisdemo --location westeurope
az group deployment create --resource-group hybrisdemo --template-file .\azuredeploy.json