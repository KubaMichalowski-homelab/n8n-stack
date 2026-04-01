# n8n-stack

This repository contains the GitOps-driven configuration for my n8n deployment. It is designed to be managed and deployed via Portainer.

## Environment Setup
The stack relies on the following environment variables:

| Variable | Description | Example |
| :--- | :--- | :--- |
| `TIMEZONE` | Sets the timezone | `Europe/Warsaw` |
| `NODE_ENV` | Optimizes the app for production performance | `production` |
| `N8N_SECURE_COOKIE` | Restricts session cookies to HTTPS only | `true` |
| `WEBHOOK_URL` | The public n8n URL | `https://n8n.domain.tld/` |

## Persistent Storage
I use bind mounts for data persistence. Ensure these paths exist on the Docker host:
* `/opt/docker/n8n` - Directory for n8n configuration

---

[Back to Homelab Overview](https://github.com/KubaMichalowski-homelab)
