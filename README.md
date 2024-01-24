# Python API in a container
Python API calc deployed in a container

Create the python app.py

Create the AKS cluster:

az login --use-device-code
az account set --subscription xxxxxx-xxxxx-xxxx-xxxx-xxxxxxxxxxxxx
az group create --name pythonapi --location eastus
az aks create --resource-group pythonapi --name pythonapidemo01 --enable-managed-identity --node-count 1 --generate-ssh-keys
