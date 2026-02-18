# ArangoDB 3.12 Docker Setup

## Quick Start

1. Start ArangoDB:
   ```bash
   docker-compose up -d
   ```

2. Access the web interface at: http://localhost:8529

3. Login credentials:
   - Username: `root`
   - Password: `rootpassword` (change this in production!)

## Commands

- **Start**: `docker-compose up -d`
- **Stop**: `docker-compose down`
- **View logs**: `docker-compose logs -f`
- **Remove data** (caution): `docker-compose down -v`

## Data Persistence

Data is persisted in Docker volumes:
- `arangodb_data` - Database files
- `arangodb_apps` - Foxx applications

## Security

⚠️ **Important**: Change the default password in production!

Edit the `ARANGO_ROOT_PASSWORD` in [docker-compose.yml](docker-compose.yml) before deploying.
