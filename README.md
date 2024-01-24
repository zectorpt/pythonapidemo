# Python API in a container
Python API calc deployed in a container <br><br>

Create the python app.py <br><br>

Create the AKS cluster: <br><br>

az login --use-device-code <br>
az account set --subscription xxxxxx-xxxxx-xxxx-xxxx-xxxxxxxxxxxxx <br>
az group create --name pythonapi --location eastus <br>
az aks create --resource-group pythonapi --name pythonapidemo01 --enable-managed-identity --node-count 1 --generate-ssh-keys <br>
