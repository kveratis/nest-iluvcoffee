# How was this project created

npm i -g @nestjs/cli
nest new
cd into directory
npm run start
npm run start:dev
nest g co // Generate controller
nest g s // Generate service
nest g mo NAME_OF_MODULE // Generate module
nest g class PATH_TO_FILE --no-spec
npm i class-validator class-transformer
npm i @nestjs/mapped-types
npm i @nestjs/typeorm typeorm pg
npx typeorm migration:create -n MIGRATION_NAME // create a new migration
npm run build // migrations need to run against compiled code
npx typeorm migration:create -n coffee-refactor
npx typeorm migration:run
npx typeorm migration:revert // to revert migrations
npx typeorm migration:generate -n schema-sync

## Examples

nest g module coffees
nest g class coffees/dto/create-coffee.dto --no-spec
nest g class coffees/dto/update-coffee.dto --no-spec
nest g class coffees/entities/flavor.entity --no-spec
nest g class common/dto/pagination-query.dto --no-spec
nest g class events/entities/event.entity --no-spec
npx typeorm migration:create -n coffee-refactor
nest g mo coffee-rating
nest g s coffee-rating
