> [!WARNING]
> This project is still work in progress we are looking for contributers to get involved so feel free to submit a pr!

# docker-rust-minecraft-server
Containerized Rust based Minecraft Java Dedicated Servers with selectable version

## Quick start

The following starts a Minecraft Java Dedicated Server with Ferrum running a default version and
exposing the default UDP port:

```sh
docker run -d -it -e EULA=TRUE -p 25565:25565/udp -v /data:/data eveeifyeve/docker-rust-minecraft-server
```

> **NOTE**: if you plan on running a server for a longer amount of time it is highly recommended using a management layer such as [Docker Compose](#deploying-with-docker-compose) or [Kubernetes](#deploying-with-kubernetes) to allow for incremental reconfiguration and image upgrades.

