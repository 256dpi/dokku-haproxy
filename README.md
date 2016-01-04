# dokku-haproxy

**haproxy tcp load balancer for dokku**

## Installation

Install the plugin:

```bash
dokku plugin:install https://github.com/256dpi/dokku-haproxy.git
```

## Configuration

Configure ports using the cli:

```bash
dokku ports:add app-name external-port process-name internal-port
```
