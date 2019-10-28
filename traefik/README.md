# Traefik / Docker Compose

The mostly difficult bit about this is the labels on the proxied container.
Traefik 2.0 documentation isn't great at the moment so these are a pain to sort out.
If you use the same .toml file and turn example-webserer.yml into docker-compose.yml in another directory, it should come up and proxy (with HTTP -> HTTPS redirect as well).
Or you can copy/paste the config and put it in the same docker-compose.yml as Traefik, just remove `network_mode: "bridge"` in that case.
