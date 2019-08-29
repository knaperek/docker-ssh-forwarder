# fodo - FOrward DOcker


This script forwards the control domain socket of a remote Docker Engine to the local machine via SSH tunnel
and sets up the local environment to talk to the remote Docker Engine.

The main objective is not to rely on Docker's TLS endpoint for remote control but instead leverage the existing
access mechanism made for this purpose - SSH. The access is easier to mange and you don't need to open up
an additional port on your firewall just for Docker access.

# Usage

```sh
$ fodo <hostname> [port]
```

# Authors
* Pavol Ivanko
* Jozef Knaperek