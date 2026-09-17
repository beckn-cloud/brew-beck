# Homebrew Tap for Beck

[![Formula](https://img.shields.io/badge/Formula-beck-blue.svg)](Formula/beck.rb)
[![Version](https://img.shields.io/github/v/release/beckn-cloud/beck)](https://github.com/beckn-cloud/beck/releases)

Homebrew formula repository for **Beck** — self-hosted PaaS CLI.

## Installation

```bash
# Add tap
brew tap beckn-cloud/brew-beck

# Install CLI
brew install beck
```

## Usage

```bash
# Verify installation
beck version

# Login to your server
beck auth login --server https://your-beck-server:8443

# Deploy an app
beck apps deploy my-api --image ghcr.io/org/api:v1 --port 8080 --regions sg
```

## Formula Details

| Field | Value |
|-------|-------|
| **Name** | `beck` |
| **Description** | Self-hosted PaaS CLI (Incus + Caddy + WireGuard) |
| **Homepage** | https://github.com/beckn-cloud/beck |
| **License** | MIT |
| **Platforms** | macOS (ARM64/Intel), Linux (ARM64/Intel) |

## Updating Formula

The formula is automatically updated by [GoReleaser](https://goreleaser.com/) when a new release is published to [beckn-cloud/beck](https://github.com/beckn-cloud/beck).

Manual update (if needed):
```bash
brew upgrade beck
```

## Uninstall

```bash
brew uninstall beck
brew untap beckn-cloud/brew-beck
```

## Related

- **Main Repo**: https://github.com/beckn-cloud/beck
- **Infrastructure**: https://github.com/beckn-cloud/beckflare
- **App Manifests**: https://github.com/beckn-cloud/beck-apps