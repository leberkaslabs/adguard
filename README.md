# AdGuard

[![CI](https://github.com/leberkaslabs/adguard/actions/workflows/ci.yml/badge.svg)](https://github.com/leberkaslabs/adguard/actions/workflows/ci.yml)

This repository contains the Docker Compose setup for AdGuard - a free and open source, powerful network-wide ads and trackers blocking DNS server.

## Requirements

- Make sure Docker and Docker Compose are installed on your system.
- Be sure to check out [AdGuard](https://github.com/AdguardTeam/AdGuardHome) - in my opinion better than Pi-hole

## Installation

The installation is straightforward. Simply clone this repository and start AdGuard using Docker Compose:

```bash
# Clone this repository
git clone https://github.com/leberkaslabs/adguard.git

# Change into repository
cd adguard

# Startup AdGuard
docker compose up -d
```

## Advanced Configuration

You can customize your setup using a Docker Compose override file:

```bash
# Create a Docker Compose override file
cp example.compose.override.yml compose.override.yml

# Recreate and apply the configuration
docker compose up -d --force-recreate
```

## License

Copyright © 2025 Niclas Spreng

Licensed under the [MIT license](LICENSE).
