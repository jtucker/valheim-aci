# Valheim Azure ACI Deployment

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjtucker%2Fvalheim-aci%2Fmain%2Fazuredeploy.json)

Or if you would like to use `az` cli in PowerShell:

``` powershell
az group create --name <resource-group> --location eastus2

az deployment group create --resource-group "<resource-group>" `
    --template-file .\azuredeploy.json `
    --parameters `@azuredeploy.parameters.json `
    --parameters valheimServerPassword yourSuperSecretPassword 

```
