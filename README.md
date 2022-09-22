# docker-nginx-proxy

A very simple container to proxy HTTP traffic to another server, based on `nginx`

## Configuration

### Environment variables

- `FORWARD_HOST` - domain of the proxied website, eg. `www.example.com`
- `FORWARD_PORT` - port of the prixied website, eg. `80`
- `FORWARD_PROT` - protocol to use for the proxied website, `http` or `https` 
- `DNS` - optionally define a nameserver for domain lookup
- `PROXY_READ_TIMEOUT` - optionally set a timeout (default 10 minutes)


See also `docker-compose.yml` file.

## Usage

With `docker-compose`

    docker-compose up -d
    
