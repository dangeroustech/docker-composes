# Proxy ARMHF

Use this for Raspberry Pi 3/4 or any other armhf platform.

# Proxying Containers

Any container that you wish to be proxied just needs the below environment variable adding to it
```
VIRTUAL_HOST=sub.domain.com
```

By default, whatever port is exposed by your container will be proxied. If you are exposing multiple ports, you can use the below to specify which one to proxy.
```
VIRTUAL_PORT=9443
```

# Usage

```
docker-compose build
docker-compose up -d
```