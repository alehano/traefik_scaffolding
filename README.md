# Traefik scaffolding for using with Cloudflare and Docker

Uses Cloudflare's Origin CA and Origin Pull certificates to secure connection.

More info:

https://developers.cloudflare.com/ssl/origin-configuration/origin-ca/
https://developers.cloudflare.com/ssl/origin-configuration/authenticated-origin-pull/set-up/zone-level/

Put your certificates into `./certs` directory:

- authenticated_origin_pull_ca.pem
- example.com.pem
- example.com.key

Change `example.com` to your domain name in all files.
Change `dynamic_conf.yml` certs names accordingly.

Run `docker-compose up -d` to start Traefik.
