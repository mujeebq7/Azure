### Commands

Check CLI version
```bash
az version
```

Login
```bash
az login
```

List subscriptions
```bash
az account list -o table
```

Show current subscription
```bash
az account show -o table
```

Show available regions
```bash
az account list-locations -o table
```

Show available VM sizes in a region
```bash
az vm list-sizes \
  --location centralindia \
  -o table
  ```

Select the appropriate subscription
```bash
az account set --subscription "<SUBSCRIPTION_ID>"
```

----
What you should understand:
- A user can have access to multiple subscriptions.
- Azure CLI operates against the currently selected subscription.
- A successful login does not guarantee permission to create resources.
- Always verify your subscription before running provisioning commands.

Official reference: https://learn.microsoft.com/en-us/cli/azure/get-started-tutorial-1-prepare-environment?view=azure-cli-latest&utm_source=chatgpt.com
