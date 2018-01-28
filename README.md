# Symfony 4 ES CQRS Boilerplate

- [x] Command Bus, Query Bus & Event Bus
- [x] Event Store
- [x] Rest API
- [x] Read Model
- [ ] Event Rest API 


### Use Cases

- [x] Register
- [x] Change Email
- [ ] Login
- [ ] Logout

## Project Setup

Up environment:
`docker-compose up -d`

Run database migrations:
`docker-compose exec php sh -lc 'dev d:m:m -n'`

Execute tests:
`docker-compose exec php sh -lc './bin/phpunit'`

Enter in php container:
`docker-compose exec php sh -l`

Disable\Enable Xdebug:
`docker-compose exec php sh -lc 'xoff'`

`docker-compose exec php sh -lc 'xon'`

### PHPStorm integration

Use ssh remote connection.

HOST: 
	- docker4mac: `localhost`
	- docker machine|| dinghy: `192.168.99.100`

PORT: `2323`

Filesystem mapping:

`{PROJECT_PATH}` -> `/app`