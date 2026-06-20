# Contributing

Thanks for your interest in LLM Stream Optimizer.

This project is in paused / limited maintenance mode, so contributions should be small, focused, and easy to review. Bug fixes, documentation improvements, and compatibility updates are more likely to be accepted than large feature additions.

## Local Setup

```bash
npm install
cp .dev.vars.example .dev.vars
npm run dev
```

Set `PROXY_API_KEY` in `.dev.vars` before using the `/admin` dashboard locally.

## Pull Request Guidelines

- Keep `worker.js` as a single-file Worker unless the change explicitly requires a larger restructuring.
- Do not commit secrets, `.dev.vars`, local Wrangler state, or generated cache files.
- Update `README.md` and `README-CN.md` together when changing setup or user-facing behavior.
- Run `npm run check` before opening a pull request.
- Describe any Cloudflare binding, secret, or compatibility-date changes in the pull request.

## Code Style

Follow the existing JavaScript style in `worker.js`. Prefer small, targeted changes over broad refactors.
