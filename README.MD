1. logga in med azure cli 'az login
2. välj rätt subscription
3. kör detta kommando 3x byt test > dev > prod


az deployment group create `
>> --resource-group RG-jamiljouj `
>> --template-file ./src/main.bicep `
>> --parameters ./src/Parameters/test.json `
>> --confirm-with-what-if `
>> --debug
