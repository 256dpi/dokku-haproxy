# dokku-haproxy

**tcp load balancer for you non-web apps**

## Installation

Install the plugin:

```bash
cd /var/lib/dokku/plugins
git clone https://github.com/256dpi/dokku-haproxy.git
dokku plugins-install
```

## Configuration

Configure ports using the cli:

```bash
$ dokku ports:add app-name external-port process-name internal-port
```
