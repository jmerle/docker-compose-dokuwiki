# Traefik DokuWiki

A Docker Compose configuration to run [DokuWiki](https://www.dokuwiki.org/dokuwiki) behind a [Traefik](https://traefik.io/) reverse proxy using [DockuWiki](https://github.com/ericbarch/dockuwiki) to support automatic backups with Git.

## Usage

1. Clone this repository.
2. Copy `.env.example` to `.env` and modify the variables.
3. Run `docker-compose up -d`.

## Installation

The first time you run it, use `docker-compose logs -f dokuwiki` to get the public SSH key that you'll need to add to the Git repository host so DockuWiki can push it's backups every hour.
