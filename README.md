# Caddy Gateway

Reverse proxy gateway powered by [Caddy](https://caddyserver.com/).

## Domains & Backends

| Domain | Proxy Target | Purpose |
|--------|-------------|---------|
| `mastersway.duckdns.org` | `localhost:8000` | General & Chat API |
| `mastersway.duckdns.org` | `localhost:7994` | Chat WebSocket |
| `mastersway.duckdns.org` | `localhost:7991` | Test WebSocket |
| `mastersway.duckdns.org` | `localhost:7996` | Notification WebSocket |
| `mastersway.duckdns.org` | `localhost:7997` | Telegram webhook |
| `trit-caddy-proxy.duckdns.org` | `localhost:13500` | Reverse proxy (with CORS) |

## Status Page

- **Deployed at:** [`trit-caddy-proxy.netlify.app`](https://trit-caddy-proxy.netlify.app)
- **Source:** [`index.html`](./index.html)
- Checks Caddy root endpoint and `/trit-universal-form` (expects 404).

## Usage

```bash
docker compose -f caddy.docker-compose.yml up -d
```