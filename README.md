# Portainer Templates 

Template + Stack to use with portainer

## Authelia:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/authelia.png" height="100"/></p>

_Authelia_ is an open-source authentication and authorization server providing two-factor authentication and single sign-on (SSO) for your applications via a web portal. It acts as a companion for reverse proxies by allowing, denying, or redirecting requests.

Documentation is available at [https://www.authelia.com/](https://www.authelia.com/).

## Heimdall:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/heimdall-icon.png" height="100"/></p>

Heimdall is an elegant solution to organise all your web applications. It’s dedicated to this purpose so you won’t lose your links in a sea of bookmarks.

Visit the website - [https://heimdall.site](https://heimdall.site).


## Nginx Proxy Manager:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/proxy_mgr.png" height="100"/></p>

This project comes as a pre-built docker image that enables you to easily forward to your websites running at home or otherwise, including free SSL, without having to know too much about Nginx or Letsencrypt.

Visit the website - [https://nginxproxymanager.com/](https://nginxproxymanager.com/).

## chowdown:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/chowdown.png" height="100"/></p>

A simple, plaintext recipe database for hackers

Visit the website - [https://chowdown.io/](https://chowdown.io/).

## wikijs:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/wikijs.png" height="100"/></p>

A modern, lightweight and powerful wiki app built on NodeJS

Visit the website - [https://js.wiki/](https://js.wiki/).

## freshrss:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/freshrss-icon.png" height="100"/></p>

FreshRSS is a self-hosted RSS feed aggregator.


Visit the website - [https://freshrss.org/](https://freshrss.org/).

## Vaultwarden:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/bitwarden.png" height="100"/></p>

Alternative implementation of the Bitwarden server API written in Rust and compatible with upstream Bitwarden clients*, perfect for self-hosted deployment where running the official resource-heavy service might not be ideal.

Visit github repository - [https://github.com/dani-garcia/vaultwarden](https://github.com/dani-garcia/vaultwarden).

## Watchtower:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/watchtower.png" height="100"/></p>

A process for automating Docker container base image updates.

Watchtower will pull down your new image, gracefully shut down your existing container and restart it with the same options that were used when it was deployed initially.

Visit the website - [https://containrrr.dev/watchtower/](https://containrrr.dev/watchtower/).

## Draw IO:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/draw-io.png" height="100"/></p>

Draw.io, this project, is a configurable diagramming/whiteboarding visualization application. draw.io is jointly owned and developed by JGraph Ltd and draw.io AG.

Visit the website - [https://www.diagrams.net/](https://www.diagrams.net/).

# Portainer Stacks 

## PiHole + Unbound:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/pihole.png" height="100"/></p>

Pi-hole® is a DNS sinkhole that protects your devices from unwanted content without installing any client-side software.

Unbound is a validating, recursive, caching DNS resolver.

This stack install piHole and couple it with Unbound.

Visit pihole website - [https://pi-hole.net/](https://pi-hole.net/).

Visit unbound website - [https://nlnetlabs.nl/projects/unbound/about/](https://nlnetlabs.nl/projects/unbound/about/).

## Duck DNS + Let's Encrypt:

<p align="center"><img src="https://github.com/Atlas34/portainer/raw/main/Images/duckdns.png" height="100"/></p>

Duck DNS : free dynamic DNS hosted on AWS

Let's Encrypt: Certbot is part of EFF’s effort to encrypt the entire Internet. Secure communication over the Web relies on HTTPS, which requires the use of a digital certificate that lets browsers verify the identity of web servers

### Environment Variables

* `DUCKDNS_DOMAIN`: Full Duck DNS domain (e.g. `test.duckdns.org`) (*required*)
* `DUCKDNS_TOKEN`: Duck DNS account token (obtained from [Duck DNS](https://www.duckdns.org)) (*required*)
* `LETSENCRYPT_DOMAIN`: Domain to generate SSL cert for. By default the SSL certificate is generated for `DUCKDNS_DOMAIN` (optional)
* `LETSENCRYPT_WILDCARD`: `true` or `false`, indicating whether the SSL certificate should be for subdomains *only* of `LETSENCRYPT_DOMAIN` (i.e. `*.test.duckdns.org`), or for the main domain *only* (i.e. `test.duckdns.org`) (optional, default: `false`)
* `LETSENCRYPT_EMAIL`: Email used for certificate renewal notifications (optional)
* `LETSENCRYPT_CHAIN`: Preferred certificate chain (e.g. `ISRG Root X1`, see [https://letsencrypt.org/certificates](https://letsencrypt.org/certificates/) for more details) (optional)
* `TESTING`: `true` or `false`, indicating whether a staging SSL certificate should be generated or not (optional, default: `false`)
* `UID`: User ID to apply to Let's Encrypt files generated (optional, recommended, default: `0` - root)
* `GID`: Group ID to apply to Let's Encrypt files generated (optional, recommended, default: `0` - root)

Visit Duck DNS website - [https://www.duckdns.org/](https://www.duckdns.org/).

Visit Let's Encrypt website - [https://github.com/certbot/certbot](https://github.com/certbot/certbot).

