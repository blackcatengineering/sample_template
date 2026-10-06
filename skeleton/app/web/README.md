# Web tier

Selected technology: `${{ values.webTechnology | default('none') }}`

Selected container/server: `${{ values.webContainer | default('none') }}`

Expected container contract:

- HTTP listens on port 8080.
- `/health` returns a successful response.
- Runtime configuration comes from environment/configuration.
- Secrets are never committed to source control.
