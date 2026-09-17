# brew-beck

Homebrew tap for [Beck](https://github.com/beckn-cloud/beck) — self-hosted PaaS CLI (Incus + Caddy + WireGuard).

## Installation

```bash
brew tap beckn-cloud/brew-beck
brew install beck
```

## Formula

| Formula | Description |
|---------|-------------|
| `beck` | Beck — self-hosted PaaS CLI for managing infrastructure and applications across multiple providers |

## Usage

```bash
# Initialize configuration
beck config init

# Login to beck-server
beck login

# Manage hosts
beck hosts list
beck hosts add my-host --endpoint=incus://host.example.com

# Deploy applications
beck apps deploy my-app --image=ghcr.io/org/app:v1 --regions=sg,jp

# Manage domains
beck domains list
beck domains add example.com --app=my-app

# View audit log
beck audit list
```

## How it works

This tap is automatically updated by [GoReleaser](https://goreleaser.com/) when a new release is published to the [beck](https://github.com/beckn-cloud/beck) repository.

The formula is generated from the `.goreleaser.yml` configuration in the main repository.