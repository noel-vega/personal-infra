# Personal Infrastructure Setup

Docker-based infrastructure with nginx reverse proxy, Let's Encrypt SSL, and private Docker registry.

## Quick Start

1. Clone this repo
2. Update `nginx.conf` - replace `registry.yourdomain.com` with your domain
3. Update `docker-compose.yml` email in certbot command
4. Set up DNS A record pointing to your server
5. Run `docker compose up -d`

## Services

- nginx: Reverse proxy with automatic HTTPS
- certbot: Automatic SSL certificate management
- registry: Private Docker registry

## Adding New Services

See [DEPLOYMENT.md](DEPLOYMENT.md) for adding new applications.
