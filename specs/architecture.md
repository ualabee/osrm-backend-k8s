# Architecture — osrm-backend-k8s

> Keep this document synchronized with the code. If code and this spec conflict, fix the spec (unless the code is wrong).

## Tech stack
- Primary language: Shell.
- Infra/container files: Dockerfile.

## Repository layout
```
Dockerfile
LICENSE
README.md
archive/
docker-entrypoint.sh
kubernetes/
tests/
```

## Modules / components
Main directories (review each directory for full details):

- `archive/` — see contents in the repository; purpose inferred from naming and README.
- `kubernetes/` — see contents in the repository; purpose inferred from naming and README.
- `tests/` — see contents in the repository; purpose inferred from naming and README.

## Data & models
No data-related environment keys detected from `.env.example`. Inspect config files for databases/queues/state.

## CI / CD
CI/CD configuration files:
- `.github/workflows/dockerhub-description.yml`

## Local development
See the repository README for run instructions; if absent, no local run steps are documented.

## Deployment
See CI workflows and infra files listed above. If deployment steps are documented in the README or `specs/`, they take precedence.

## Testing
Test locations: `tests/`.
