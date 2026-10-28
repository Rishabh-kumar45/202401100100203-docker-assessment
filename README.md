# Docker & Container Security Assessment

## Student Details

- Name: Rishabh Kumar
- Registration Number: 202401100100203
- Port: 8083
- Docker Hub Username: rishabh0145

## Repositories

- GitHub: https://github.com/Rishabh-kumar45/202401100100203-docker-assessment
- Docker Hub: https://hub.docker.com/r/rishabh0145/fest-backend

## Application Architecture

FestPass consists of three services:

- Frontend: Nginx
- Backend: Python Flask
- Database: PostgreSQL

Docker Compose connects the frontend and backend through
one network and the backend and database through another.

PostgreSQL data is stored in a named Docker volume.

## Image Versions

- fest-backend:0.1 — Initial image
- fest-backend:0.2 — Hardened image
- rishabh0145/fest-backend:1.0.0 — Published and signed release
- rishabh0145/fest-backend:1.0 — Additional version tag
- rishabh0145/fest-backend:1.0.1 — Published unsigned test release

## Docker Image Digest

Record the actual digest returned when version 1.0.0
was pushed to Docker Hub.

- Digest: sha256:cf49841ed2585358f88a3d56656b262cfffa1f107a348a19417444ead2448e25

## Vulnerability Comparison

| Measurement | Before (0.1) | After (0.2) |
|---|---:|---:|
| Critical vulnerabilities | Fill actual result | Fill actual result |
| High vulnerabilities | Fill actual result | Fill actual result |
| Image size | Fill actual result | Fill actual result |

## Image Security

- Trivy was used to scan both backend images.
- The hardened backend runs as a non-root user.
- Cosign was used to sign version 1.0.0 by digest.
- The signature was verified using cosign.pub.
- Version 1.0.1 was published without signing and its
  verification was tested.

## AI Tools

ChatGPT was used help draft,
Docker configuration, suggest commands, and troubleshoot
errors. All commands were executed and checked by me.
