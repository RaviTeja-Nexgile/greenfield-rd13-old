# Tasks: Leave Tracker

- [x] 1. Project setup
  - The Node.js server with GET /api/health, and its test.
  - _Requirements: 1.1_
  - _Files: package.json, package-lock.json, src/**, test/**_
  - _Verify: npm test_
- [x] 2. Deployment setup
  - Write what ssh-docker needs to build and run the app on the server, and do not deploy it: a Dockerfile, a .dockerignore and docker-compose.prod.yml.
  - _Requirements: 1.1_
  - _Depends: 1_
  - _Files: Dockerfile, .dockerignore, docker-compose.prod.yml_
  - _Verify: docker compose -f docker-compose.prod.yml config --quiet --no-interpolate_
  - _Verify: docker build -t leave-tracker-old:verify ._
  - _Mode: devops_

- [ ] 3. Deployment setup for Fly.io
  - Write what Fly.io needs to build and run the app there, and do not deploy it: for example its configuration file, a Dockerfile, or the workflow of a pipeline that deploys it.
  - Read every secret from an environment variable. Never write a secret in a file.
  - _Requirements: 1.1_
  - _Files: **_
  - _Verify: npm test_
  - _Mode: devops_
