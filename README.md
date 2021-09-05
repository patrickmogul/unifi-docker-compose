# Unifi Controller via Docker Compose
Docker Compose files to run a Unifi Controller based off of https://github.com/jacobalberty/unifi-docker images

### Requirements
- docker
- docker-compose

### Install
```bash
git clone https://github.com/easy-node-one/unifi-docker-compose.git
cd unifi-docker-compose
docker-compose up -d
```

### Upgrade
```bash
docker-compose pull
docker-compose down
docker-compose up -d
```

### Features
- Persistent storage in the docker-compose folder
- MongoDB can't run with local storage on windows so it uses a volume
    - If you're on linux, set up the MongoDB volume locally for persistent DB