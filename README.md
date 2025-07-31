# GeoIP-based SSH Access Filter

This package provides a GeoIP-based SSH access filter for Ubuntu, allowing you to allow or deny SSH connections based on the client's country. It is based on the scripts described in [this article](https://www.claudiokuenzler.com/blog/676/ssh-access-filter-based-on-geoip-database-allow-deny) by Claudio Kuenzler.

## Features

- Automatically filters SSH connections by country code
- Uses GeoIP database for IP geolocation

## Installation

1. Download the `.deb` package from the Releases section
2. Install with:
   ```bash
   sudo apt install ./geossh.deb
   ```

## Configuration

Edit `/usr/local/bin/ipfilter.sh` to set:
- `ALLOW_COUNTRIES` - space-separated list of allowed country codes (e.g., "CH DE US")
- `ALLOW_IPS` - space-separated list of whitelisted IP addresses (default 127.0.0.1)
