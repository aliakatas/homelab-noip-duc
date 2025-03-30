# Homelab NoIP-DUC
Utility to keep the DNS record up-to-date using Dynamic Update Client from NoIP for Linux (using Docker).

A useful guide can be found through the [official channel](https://github.com/noipcom/linux-update-client-docker).

To deploy, make sure to create a `.env` file with the following information as a minimum:
```
NOIP_USERNAME={}
NOIP_PASSWORD={}
NOIP_HOSTNAMES={}
```

To explore other options, run the following:
```bash
docker run -it ghcr.io/noipcom/noip-duc:latest --help
```

If multiple DNS hostnames need to be updated using the same host, make sure to update the `.env` file before running the container.
