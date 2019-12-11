# Introduction 
Choosing your vm size.

# Getting Started
The simple way is to choose from general compute, the latest generation and a common amount of internal memory, like Standard_D2s_v3 (which allow for premium storage and caching)

1.	Diving a bit deeper

There are other compute types. For instance the Dv3 series has a 1:4 core-to-memory ratio. Memory-optimized vm types have more memory relatively (like 1:8) and compute-optimized has more cores (like 1:2). More info on [vm sizes](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/sizes).

To get a list of available vm sizes in your region:
```
az vm list-skus --query "[].{name:name}" --location $region -o table
```

2. Going even deeper

There are additional resources that can help select the best performance and price:

[Compute benchmark scores](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/compute-benchmark-scores) provide an average ***performance*** score for each of the vm sizes. 

And [Azure VM Comparison](https://azureprice.net/) gives you a list of vm sizes, with filtering and sorting including ***prices***, which can give you the cheapest option for instance for a vm with 8 gb internal memory in westeurope. 

With all of this combined, you can really make an informed decision.

# Contribute
Feel free to contribute. Create an issue or pull request.  

