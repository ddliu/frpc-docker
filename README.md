# frpc-docker
frpc(frp client) docker build

This tiny(only 7.3MB) frpc image is built with busybox.

Usage:

```
docker run -v /path/to/frpc.ini:/etc/frpc.ini ddliu/frpc
```

Basic frpc.ini config:

```ini
[common]
server_addr = x.x.x.x
server_port = 7000

[ssh]
type = tcp
local_ip = x.x.x.x (maybe host IP)
local_port = 22
remote_port = 6000
```

[Looking for frps build?](https://github.com/ddliu/frps-docker)
