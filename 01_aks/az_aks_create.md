# Introduction 
This is a walkthrough of creating an Azure Kubernetes Cluster through the command-line interface.

# Getting Started
The easiest way to do this is to use the Azure cloud shell, either available through the icon at the top bar in the [Azure portal](https://portal.azure.com) or at https://shell.azure.com

1.	Installation process
```
resourcegroupname=aksrg
region=westeurope
az group create --name=$resourcegroup --location=$region

```

2.	Software dependencies
All dependencies are managed by the Azure cloud shell, so no need to do anything. If you want to do this the hard way, follow instructions in references below at aks create walkthrough. 

# Build and Test
TODO: Ideally we get to a point where the cluster creation is automated and also testing is automated. 

# Contribute
Feel free to contribute. Create an issue or pull request.  

# References
- [az aks create](https://docs.microsoft.com/en-us/cli/azure/aks?view=azure-cli-latest#az-aks-create)
- [aks best practices](https://docs.microsoft.com/en-us/azure/aks/best-practices)
- [aks networking](https://docs.microsoft.com/en-us/azure/aks/concepts-network)
- [aks create walkthrough](https://docs.microsoft.com/en-us/azure/aks/kubernetes-walkthrough)