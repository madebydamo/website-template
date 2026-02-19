# Website Template

Simple Dockerized static website template for beginners.

## Dependencies

- [Docker](https://docs.docker.com/get-docker/)
  - [Linux](https://docs.docker.com/engine/install/)
  - [Windows](https://docs.docker.com/desktop/install/windows-install/)
  - [macOS](https://docs.docker.com/desktop/install/mac-install/)

## Quickstart

1. Fork this repo on GitHub: https://github.com/anomalyco/website-template/fork
2. Clone your fork: `git clone https://github.com/YOURUSERNAME/website-template.git`
3. `cd website-template`
4. Edit files in `www/`
5. Start dev server: `docker compose up -d` (live reload at http://localhost:8000)
6. Stop: `docker compose down`

## Build & Publish to DockerHub

1. Create [DockerHub](https://hub.docker.com/) account & `docker login`
2. `IMAGE_NAME=yourusername/website docker compose build`
3. `docker push yourusername/website`

## Git Workflow

Make changes, `git add .`, `git commit -m "Update homepage"`, `git push origin master`

## Production

Build image as above, run without compose volumes to use baked-in files.
