# dokku-haproxy

**haproxy tcp load balancer for dokku**

## Installation

Install the plugin:

```bash
dokku plugin:install https://github.com/256dpi/dokku-haproxy.git
```

### Installation Notes
 * This plugin will expose the stats interface on port 9090, its up to you to allow or block this port in your firewall.
 * This plugin requires a Dokku version of 0.4.x or higher. 0.5.x is highly recommended. SEE: [Upgrading Dokku](https://github.com/dokku/dokku/blob/master/docs/upgrading.md).

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
