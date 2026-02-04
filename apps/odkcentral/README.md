# ODK Central for Runtipi

This app deploys **ODK Central** with PostgreSQL and Redis, fully managed by Runtipi.

## Features

- HTTPS via Traefik
- Persistent storage for Postgres and Central
- Sysadmin setup via install form
- Multi-architecture support: amd64, arm64

## Installation

1. Open your Runtipi custom store
2. Find **ODK Central**
3. Fill the install form (hostname, credentials)
4. Click **Install**
5. Wait for Traefik to provision HTTPS
6. Access ODK Central at your chosen hostname

## Notes

- Do not manually run `docker-compose up` unless top-level volumes exist
- Recommended: pin `getodk/central` image to a stable release for production
