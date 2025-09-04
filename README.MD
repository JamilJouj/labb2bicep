1. logga in med azure cli `az login`
2. välj rätt subscription
3. kör detta kommando 3x byt test > dev > prod

```shell
az deployment group create `
  --resource-group <YourResourceGroupName> `
  --template-file ./src/main.bicep `
  --parameters ./src/Parameters/dev.json `
  --confirm-with-what-if 
```
