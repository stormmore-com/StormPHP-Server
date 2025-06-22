# StormPHP Server
It's a simple server designed to work with the StormPHP Framework.\
Easy and lightweight, with everything you need to go into production.

### Running StormPHP Server
Run `storm-server`. By default, it serves files from the working directory on port  80.

### Download link
[Windows](https://github.com/stormmore-com/storm-server/releases/download/0.1.0/storm-server.x64.zip)\
[MacOS (intel)](https://github.com/stormmore-com/storm-server/releases/download/0.1.0/storm-server.macos.intel.zip)

**Features**
- Listing directory
- Serving files
- HTTP/HTTPS
- Load balancing

**Coming next**

- FastCGI/PFM integration
- StormPHP Framework integration
- Windows/MacOS/Linux installers

### Configuration
Run storm-server with the parameter
`storm-server -f config.txt`

### Example configuration file

```
dir = /path/to/your/directory
port = 87
timeout = 30

logs.enabled = yes
logs.min_level = debug

https.enabled = yes
https.public_key = yours_public_key.pem
https.private_key = path_to_yours_public_key.pem

load_balancer.enabled = yes
load_balancer.servers = 127.0.0.1:100
load_balancer.servers = 127.0.0.1:101
load_balancer.servers = 127.0.0.1:102
```