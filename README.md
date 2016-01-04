# dokku-haproxy

**haproxy tcp load balancer for dokku**

## Installation

Install the plugin:

```bash
dokku plugin:install https://github.com/256dpi/dokku-haproxy.git
```

_Note: This plugin will expose the stats interface on port 9090, its up to you to allow or block this port in your firewall._

## Usage

The plugin offers the following commands via the dokku tool:

```
ports:add <app> <eport> <proc> <iport> Add a port configuration
ports <app>                            Display configured ports
ports:remove <app> <eport>             Remove a port configuration
```

To add a port configuration, run the following example command:

```bash
dokku ports:add my-app 80 web 8080
```

To remove that configuration later, run the following example command:

```bash
dokku ports:remove my-app 80
```
