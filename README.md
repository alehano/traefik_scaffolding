# Traefik scaffolding for using with Cloudflare and Docker

Uses Cloudflare's Origin CA and Origin Pull certificates to secure your Traefik dashboard and API.

More info:

https://developers.cloudflare.com/ssl/origin-configuration/origin-ca/
https://developers.cloudflare.com/ssl/origin-configuration/authenticated-origin-pull/set-up/zone-level/

Put your certificates into ssl directory by the following names:

- cloudflare-origin-cert.pem
- cloudflare-origin-key.pem
- authenticated_origin_pull_ca.pem

Run `docker-compose up -d` to start Traefik.
