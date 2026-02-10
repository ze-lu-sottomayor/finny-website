# Finny Website

Landing page for [finnybot.com](https://finnybot.com) — Your AI Personal Finance Bot on Telegram.

## Stack

- Static HTML/CSS (no build step)
- Nginx (Alpine) for serving
- Kamal for deployment
- Traefik for SSL/routing

## Local Development

```bash
# Just open index.html in a browser, or:
docker build -t finny-website .
docker run -p 8080:80 finny-website
```

## Deploy

```bash
kamal setup    # First time
kamal deploy   # Updates
```

## Structure

```
├── index.html          # Landing page (SEO-optimized)
├── styles.css          # Styles
├── favicon.svg         # Favicon
├── nginx.conf          # Nginx config
├── Dockerfile          # Container build
├── config/deploy.yml   # Kamal deployment config
└── .github/workflows/  # CI/CD
```
