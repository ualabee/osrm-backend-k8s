# AGENTS.md — osrm-backend-k8s

Agent operating guide for `osrm-backend-k8s`. This repository is iterated by AI agents; this file is the index that relates every spec in `specs/` and defines how agents should act.

## Overview

Open Source Routing Machine (OSRM) osrm-backend for Kubernetes on Google Container Engine (GKE).

## Spec index

- [specs/README.md](specs/README.md) — catalog of all specs and their purposes.
- [specs/product-overview.md](specs/product-overview.md) — business context, value, customers, and ecosystem relationships.
- [specs/architecture.md](specs/architecture.md) — tech stack, databases, models, modules, CI, local development, deployment, and testing.

## Agent operating rules

1. **Preserve external constants.** Database names, connection hosts, Firebase/GCP/Azure resource IDs, city IDs, API base URLs, bucket names, and any configuration coming from services or projects outside this repository must be kept exactly as-is. Never invent replacements.
2. **Keep specs truthful.** Specs and code must never conflict. After any material change, update the affected specs and this file in the same session.
3. **World-class code quality.** Match existing patterns, handle errors explicitly, add/update tests when this repository's practice expects them, and avoid unrelated refactors.
4. **Security.** No secrets in source, logs, or specs. Use environment variables/secret managers already used by the product; preserve authN/authZ and multi-tenant isolation; validate inputs at trust boundaries; prefer least privilege.
5. **UX/UI (where this repo has a UI).** Meet world-class UX/UI standards: clear hierarchy, accessible contrast/focus, responsive layout, consistent spacing/typography, and complete loading/empty/error states.
6. **English only.** Code, comments, specs, and commits in English, except user-facing strings/translations.
7. **Parallelize.** Use parallel subagents for independent analysis, domains, or modules.
8. **Local run, CI, deploy, testing.** See [specs/architecture.md](specs/architecture.md) and the repository README.

## Quick start

> # osrm-backend for Kubernetes [![](https://images.microbadger.com/badges/image/peterevans/osrm-backend-k8s.svg)](https://microbadger.com/images/peterevans/osrm-backend-k8s) [![CircleCI](https://circleci.com/gh/peter-evans/osrm-backend-k8s/tree/master.svg?style=svg)](https://circleci.com/gh/peter-evans/osrm-backend-k8s/tree/master) Open Source Routing Machine (OSRM) [osrm-backend](https://github.com/Project-OSRM/osrm-backend) for Kubernetes on Google Container Engine (GKE). This Docker image and sample Kubernetes configuration files are one solution to persisting [osrm-backend](https://github.c
