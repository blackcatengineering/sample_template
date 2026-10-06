# Architecture

## Selected components

Web: `${{ values.webEnabled }}` / `${{ values.webTechnology | default('none') }}`

API: `${{ values.apiEnabled }}` / `${{ values.apiTechnology | default('none') }}`

Database: `${{ values.databaseEnabled }}` / `${{ values.databaseTechnology | default('none') }}`

Database hosting: `${{ values.databaseHosting | default('none') }}`

Deployment: `${{ values.deploymentTarget }}`

Cloud: `${{ values.cloudProvider }}`

## Runtime boundaries

```text
Browser
   |
   v
Web tier
   |
   v
API tier
   |
   v
Data tier
```

The web tier should not connect directly to the database.
