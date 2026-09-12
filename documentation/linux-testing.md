# Linux Testing

## Tool
Docker Desktop

## Environment
Ubuntu 24.04 LTS container

## Initial Issue
The Docker command failed because the Docker daemon was not running.

Error:
docker: failed to connect to the docker API

## Troubleshooting
1. Started Docker Desktop.
2. Ran `docker info` to confirm the Docker server was available.
3. Verified the environment reported Linux and aarch64 architecture.
4. Launched an Ubuntu 24.04 container successfully.

## Validation
Ran:
- `uname -a`
- `cat /etc/os-release`

Result:
PASS — Ubuntu 24.04.4 LTS launched successfully.

## What I Learned
I practiced identifying an environment issue, verifying the Docker service, and validating a Linux test environment.
