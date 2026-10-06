# API tier

Selected technology: `${{ values.apiTechnology | default('none') }}`

Expected container contract:

- HTTP listens on port 8080.
- `/health` returns a successful response.
- `/ready` reports readiness.
- Database credentials are supplied as secrets.
- Runtime configuration comes from environment/configuration.
