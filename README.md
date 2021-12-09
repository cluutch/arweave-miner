# Readme

**NOTE:** Here be 🐉 dragons, this is early testing software.

## Quickstart

1. Install Docker and Docker Compose.
2. On the host, set the following values in `/etc/sysctl.conf`.

```
fs.file-max=900000
fs.nr_open=9000001
```
3. `docker-compose up`
4. Wait a few minutes, and then query the system: `curl localhost:1984/info`


## Workflow Status

| Status | Description |
| :----- | :---------- |
| ![Dependabot](https://api.dependabot.com/badges/status?host=github&repo=salt-labs/arweave-miner) | Automated dependency updates |
| ![Greetings](https://github.com/salt-labs/arweave-miner/workflows/Greetings/badge.svg) | Greets new users to the project. |
| ![Docker](https://github.com/salt-labs/arweave-miner/workflows/Docker/badge.svg) | Testing and building containers with Docker |
| ![Labeler](https://github.com/salt-labs/arweave-miner/workflows/Labeler/badge.svg) | Automates label addition to issues and PRs |
| ![Release](https://github.com/salt-labs/arweave-miner/workflows/Release/badge.svg) | Ships new releases :ship: |
| ![Stale](https://github.com/salt-labs/arweave-miner/workflows/Stale/badge.svg) | Checks for Stale issues and PRs  |

## Description

Container image for mining ⛏️ on the Arweave Network.

# via: https://docs.docker.com/engine/install/ubuntu/
Install Docker on server

```
apt update
apt upgrade
apt autoremove

apt-get remove docker docker-engine docker.io containerd runc

apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```