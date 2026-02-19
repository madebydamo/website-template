# Agent Instructions

## Overview
Static HTML/JS/CSS site served via Python HTTP server in Docker (port 8000).

## Dev Server
`docker compose up -d` mounts `./www:/app`, edits live at http://localhost:8000.
`docker compose down` to stop.

## Build
`IMAGE_NAME=foo docker compose build` (copies www/ into image).
Run prod: `docker run -p 8000:8000 IMAGE_NAME`.

## No Tests/Lint
None required.

## Files
- www/: static files
- Dockerfile: Python server
- docker-compose.yml: dev/prod build

Verify: `docker compose up --build` & check localhost:8000.