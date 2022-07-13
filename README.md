# Byjus-learning - SOS and Achieve
## Start the nucleus-gateway
npx --userconfig .npmrc  @byjus-orders/nucleus-gateway -l so

## Generating a migration script
npm run migration:generate -- --name [schema_action_resource_name.js] --skip-verify 
## Test DB migration in local machine
**up**  &emsp =>   npm run db:migrate -- --name 2022.07.13T13.39.06.schema_action_resource_name.js <br>
**down** &emsp &nbsp  =>   npm run db:migrate:undo -- --name 2022.07.13T13.39.06.schema_action_resource_name.js


## General instructions
1. Use import statements for the public/global libraries on top 
2. Use private imports in the end just for structurising
3. Always give default values