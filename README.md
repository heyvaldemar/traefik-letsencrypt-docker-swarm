# Traefik with Let's Encrypt in a Docker Swarm

Install the Docker Engine by following the official guide: https://docs.docker.com/engine/install/

Install the Docker Swarm by following the official guide: https://docs.docker.com/engine/swarm/swarm-tutorial/create-swarm/

Create a network for Traefik before deploying the configuration using the command:

`docker network create -d overlay traefik-network`

Deploy Traefik in a Docker Swarm using the command:

`docker stack deploy -c traefik-letsencrypt-docker-swarm.yml traefik`
