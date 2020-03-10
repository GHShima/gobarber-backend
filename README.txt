yarn install
yarn dev 

docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

yarn sequelize db:migrate
yarn sequelize db:migrate:undo
yarn sequelize db:migrate:undo:all