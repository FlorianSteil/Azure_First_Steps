# Azure CLI

## Install CLI

1. [How to install the Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli?WT.mc_ID=MSIgnite-session-pierrer)

1. Open Powershell or Terminal
1. Enter the following command: <code>az login</code>
1. Set your subscription if you manage multiple subscriptions: code>az laccount set --subscription 'yoursub'</code>

## Create first web app

1. Create Resourcegroup: <code>az group create --location westeurope --name test1</code>
1. Create App service plan: <code>az appservice plan create --name TestWebServicePlan --resource-group test1 --sku FREE</code>
1. Create WebApp <code>az webapp create --name "FirstDemoWebApp" --resource-group test1 --plan TestWebServicePlan</code>
