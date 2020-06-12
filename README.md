# Kubernetes
Repo to house Kubernetes learning tools/material

Kubernetes/Azure Cheat Sheet
Resources
WINDOWS
·        AZURE CLI (AZ CLI)
https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-windows?view=azure-cli-latest
·        KUBENETES CLI (kubectl)
https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-windows
·        HELM
https://github.com/helm/helm/releases/tag/v2.14.1
·        VSCode
https://code.visualstudio.com/download
 
Mac
·        AZURE CLI (AZ CLI)
https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-macos?view=azure-cli-latest
·        KUBENETES CLI (kubectl)
https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-macos
·        HELM
https://github.com/helm/helm/releases/tag/v2.14.1
·        VSCode
https://code.visualstudio.com/download
Commands
Azure

Login with your Microsoft Account
az login

List subscriptions once logged in
az account list -o table

Set the correct subscription
az account set --subscription "<subscription_name>"

Download the AKS Kube Cluster config file to the local config file
az aks get-credentials --resource-group "USE CLOUD SLICE ASSIGNED RESOURCE GROUP" --name aks-k8s-cluster


Kubernetes
Create a pod using YAML File
kubectl apply -f simple-pod.yaml

List running pods
kubectl get pods

Access pods
kubectl port-forward nginx-pod 8001:80


