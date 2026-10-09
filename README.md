# Caddy Gateway

Reverse proxy gateway powered by [Caddy](https://caddyserver.com/).

## Domain & Backend

| Domain | Proxy Target |
|--------|-------------|
| `trit-caddy-proxy.duckdns.org` | `localhost:13500` |

## Status Page

- **Deployed at:** [`trit-caddy-proxy.netlify.app`](https://trit-caddy-proxy.netlify.app)
- **Source:** [`index.html`](./index.html)

## Usage

```bash
docker compose -f caddy.docker-compose.yml up -d
```