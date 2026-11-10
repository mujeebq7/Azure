### Create a resource group

We will create a resource group for a fictional healthcare application.

```bash
export LOCATION="centralindia"
export RG="rg-lab"
az group create --name "$RG" --location "$LOCATION"
```

Verify:
```bash
az group list -o table

az group show --name "$RG" -o json
```

Expected result:
```bash
Name             Location
---------------  -------------
rg-lab    centralindia
```
----

Question: 

Why would an organization separate production and development resources into different resource groups or subscriptions?

Expected answer: 

Isolation, access control, resource lifecycle management, cost attribution, and governance. Subscription separation may provide stronger billing and security boundaries.
