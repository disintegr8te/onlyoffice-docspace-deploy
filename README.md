# ONLYOFFICE DocSpace - Kanzlei Fahlenbock

Self-hosted ONLYOFFICE DocSpace deployment for **Rechtsanwaltin Sabrina Fahlenbock**.

## Access

- **URL:** https://docspace.fahlenbock-cloud.net
- **Hosted on:** Coolify (Hetzner Cloud)

## Architecture

Consolidated Docker Compose with ~20 services:
- **Infrastructure:** MySQL 8.3, Redis 7, RabbitMQ 3
- **Document Server:** ONLYOFFICE Docs (Community Edition)
- **DocSpace Services:** API, Files, Studio, Login, SSO, Backup, etc.
- **Router:** Internal nginx routing
- **Proxy:** nginx with Traefik labels for SSL termination

## Deployment

Deployed via Coolify docker-compose. Traefik handles SSL (Let's Encrypt).

## Branding

Branded for Kanzlei Fahlenbock:
- Colors: Sage Green (#8FA898), Charcoal (#2B2B2B), White
- Font: Inter
- Tagline: "Klar. Prazise."
