# TypeScript + Hapi = <3

This is a super simple starter kit to develop APIs with HapiJS + TypeScript

## What currently supports? 

This starter kit comes with the following features: 

- **Swagger-UI** 
- **Status Monitor**
- **.env files support**
- **ts-node-dev for hot-reload**
- **Pretty Console Logger with Winston** 
- **Work with Yarn or NPM 6 as dependency resolvers**
- **Code formatting with Prettier as hook for Pre-commit**
- **Dockerfile + docker-compose for development**
- **Basic Test Suite with Tape**
- **Coverage Report**
- **Supports Heroku Deployment**

## Requirements

* NodeJS 10.x

## How to use it? 

1. Download this project as a zip.
2. Run `npm install`
3. Run `npm run dev`
4. Visit [http://localhost:8080/documentation](http://localhost:8080/documentation) to view swagger docs.
5. Visit [http://localhost:8080/api/users](http://localhost:8080/api/users) to test the REST API.
6. Visit [http://localhost:8080/status](http://localhost:8080/status) to view the status monitor.

## How to debug?
1. Install Visual Studio Basic
2. Place the break points in Visual Studio Basic
3. Run your code in debug `Build Project` environment.

## TODO

This is not finished, there's still a lot of things to improve. Here you got some:

- [X] Simple test suite - added by the help of [@jcloutz](https://github.com/jcloutz)
- [X] Add support for test coverage - added by the help of [@jcloutz](https://github.com/jcloutz)
- [ ] Add Socket.io for real time event send and receive.
- [ ] Add GraphQL support
- [ ] Add support for Auth with JWT or Sessions
- [ ] Add support for TypeORM/Mongoose
- [ ] Add support for Jenkins pipeline

## Documentation

### What are the package.json scripts for?

* `build`: Compiles typescript based on config set in tsconfig.json.
* `start`: Starts node with the compiled typescript. Used by eg. Heroku.
* `prestart`: Automatically create the js build from ts files
* `dev`: It hot reload the project on ts file changes.
* `docker:logs`: View Docker logs
* `docker:ps`: List Docker containers
* `docker:start`: Start Docker container based on docker-compose.yml file.
* `docker:stop`: Stop Docker container
* `format:lint`: Runs tslint on the typescipt files, based on tslint.js settings.
* `format:prettier`: Runs prettier on all ts-files.
* `postinstall`: Runs build-ts script. This is used by eg. Heroku automatically.
* `test`: Runs tests using nyc, and creates coverage report.

## Contributing

Of course, if you see something that you want to upgrade from this library, or a bug that needs to be solved, PRs are welcome!

## This repository is cloned from 

https://github.com/BlackBoxVision/typescript-hapi-starter