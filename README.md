# Development Environment

A development environment containing docker containers for common services, e.g. PostgreSQL

## Services

| Service | Port(s) | Command | Notes |
| ------- | ---- | ------- | ----- |
| Postgres | `5432` | `npm run db` | Database |

## Development

### Prerequisites

* [NodeJS](htps://nodejs.org), version 11+ (I use [`nvm`](https://github.com/creationix/nvm) to manage Node versions — `brew install nvm`.)
* [Docker](https://www.docker.com) (Use [Docker for Mac](https://docs.docker.com/docker-for-mac/), not the homebrew version)

### Initialisation

    npm install

### To start Postgres

First ensure nothing else is using port `5432`

    npm run db

### To stop them all

    npm run stop:all

### To kill them all and wipe all development data

    npm run kill:all