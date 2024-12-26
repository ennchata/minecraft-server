# minecraft-server

A simple docker based Minecraft server for my friends, made into a git repository for safekeeping.

Uses the following images:
| Image | Purpose |
| :-- | :-- |
| [itzg/minecraft-server](https://hub.docker.com/r/itzg/minecraft-server) | Minecraft server |
| [nginx](https://hub.docker.com/_/nginx) | Compact browser frontend |
| [Traefik](https://hub.docker.com/_/traefik) | Routing (configuration not included in repository) |

Run the stack with `docker compose up` (after creating a common network for Traefik routing with `docker network create proxy`). You can access the Minecraft server CLI with `docker exec -it <container_id> rcon-cli`.

