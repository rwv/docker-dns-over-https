# docker-dns-over-https
Dockerized [m13253/dns-over-https](https://github.com/m13253/dns-over-https)

## Quick Start

The following commands use default configuration from [m13253/dns-over-https](https://github.com/m13253/dns-over-https).

Run doh-client

``` sh
$ docker run -d -p 53:53 seedgou/dns-over-https /doh-client
```

Run doh-server

``` sh
$ docker run -d -p 8053:8053 seedgou/dns-over-https /doh-server
```

## Mount Configuration

Replace `~/doh-client.conf` with your configuration path.

``` sh
$ docker run -d -p 53:53 -v ~/doh-client.conf:/doh-client.conf seedgou/dns-over-https /doh-client
```

