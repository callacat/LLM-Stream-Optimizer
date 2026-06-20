# Security Policy

## Maintenance Status

LLM Stream Optimizer is currently in paused / limited maintenance mode. Security fixes are not guaranteed on a fixed timeline, so production users should review the code and Cloudflare configuration before deploying.

## Supported Versions

The repository does not currently maintain separate release branches. Use the latest commit on `main` if you choose to self-host the project.

## Secret Handling

- Never commit `.dev.vars`, production API keys, dashboard passwords, or other secrets.
- Use a strong `PROXY_API_KEY`; it is used both as the proxy API key and as the `/admin` dashboard password.
- Prefer Cloudflare Worker secrets for production credentials.
- Treat KV data as sensitive because it may contain upstream API configuration.

## Reporting a Vulnerability

If you find a vulnerability, please open a private report through GitHub security advisories if available, or contact the repository owner through GitHub. Include enough detail to reproduce the issue, affected routes, and any relevant Cloudflare Worker configuration.

Because maintenance is limited, please avoid publishing exploit details before the maintainer has had a reasonable chance to respond.
