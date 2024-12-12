# Docker Compose Stack for Nextcloud All-in-One behind Tailscale
*Based on https://github.com/nextcloud/all-in-one/discussions/5439.*

The purpose of this Docker Compose stack is to allow serving Nextcloud AIO without a need neither for a public IP address nor for an own domain. Tailscale's [MagicDNS](https://tailscale.com/kb/1081/magicdns) is used for this purpose.

Services:
1. **nextcloud-aio-mastercontainer** - The official [Nextcloud](https://github.com/nextcloud/all-in-one) installation method.
2. **nextcloud-caddy** - Reverse proxy sidecar.
3. **nextcloud-tailscale** - Tailscale sidecar.
