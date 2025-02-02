# ${{ values.title }}

## How to setup

- Node
  - Run `yarn` to install dependencies
- Environment variables
  - Copy `env.example` to a new `.env` file
  - Fill/replace `.env` with the required credentials
- Docker
  - Create a `docker-compose.override.yml` if you want to change something of `docker-compose.yml`
  - Run `yarn docker:build` to build the API into a new docker image
  - Run `yarn docker:up` to set up all containers
- Migrations:
  - Run `yarn migration:up` to generate postgresql database structure

## How to run

- Run `yarn start:dev`

## How to build

- Run `yarn build`

## How to deploy

- Every push to the `develop` branch will trigger a GitHub CI workflow. This workflow is available under the `./.github/workflows` directory. Once ran, the code will be deployed on the server

## Links

- [${{ values.title }}](${{ values.url }})
- [${{ values.title }} Insomnia](${{ values.insomniaUrl }})
- [${{ values.title }} Swagger](${{ values.url }}/api)
