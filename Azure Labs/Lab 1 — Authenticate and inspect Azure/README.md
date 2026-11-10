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
