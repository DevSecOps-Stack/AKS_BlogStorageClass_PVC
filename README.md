# aks-storage-class-pvc

az group create --name AKSRG --location eastus

az acr create --resource-group AKSRG --name aksreg --sku Basic

az aks create -g AKSRG -n testproj --location eastus --attach-acr akscontainerhub --generate-ssh-keys
