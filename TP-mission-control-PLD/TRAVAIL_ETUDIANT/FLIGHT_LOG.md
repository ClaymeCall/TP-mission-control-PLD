# ORBITER-7 - Flight Log

## Crew

- Builder:
- Flight Controller:
- Safety Officer:

## Gate 01 - Baseline and optimization

| Metric | Baseline | Final | Improvement |
|---|---:|---:|---:|
| Image size | 371.8MB | 46.7MB | -87.4% |
| Full build time | 11.5s | 10.3s | -1.2s |
| Code-only rebuild time | 11.5s | 2.5s | -9.0s (cache) |

- Baseline running user:
- Final running user:
- What changed and why: nous avons changé l'image de base de `node:20` vers `node:20-alpine` et optimisé le Dockerfile (cache des dépendances via `COPY package*.json` + `npm ci` et ajout de `Dockerfile.dockerignore`) ; la taille de l'image a évolué de 371.8MB à 46.7MB et le temps de rebuild avec cache a évolué de 11.5s à 2.5s.

## Gate 02 - Container safety

- `docker inspect` health status:
- Evidence that PID 1 is not root:
- Healthcheck command used:

## Gate 03 - Continuous Integration

- First successful workflow run:
- Failing pull request run:
- Fixed pull request run:

## Gate 04 - Compatibility and cache

- Runtime versions tested:
- Cache-hit run:
- Time before cache:
- Time after cache:

## Gate 05 - Security clearance

- Trivy run:
- Blocking severity policy:
- Critical findings at ship time:

## Gate 06 - Registry and release

- GHCR package URL:
- `latest` tag:
- SHA tag:
- Optional version tag:

## Final crew note

In 5 lines maximum: what made the biggest difference between "it runs" and "we can ship it"?
