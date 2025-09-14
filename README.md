# SynoDeploy Homebrew Formula

Official Homebrew formula for [SynoDeploy](https://github.com/scttfrdmn/synodeploy) - a CLI tool for deploying containers to Synology DSM 7.2+.

## Installation

```bash
# Add the tap
brew tap scttfrdmn/synodeploy

# Install synodeploy
brew install synodeploy

# Verify installation
synodeploy --version
```

## Usage

```bash
# Setup connection to your Synology NAS
synodeploy init your-nas.local --user your-username

# Deploy a container
synodeploy run nginx:latest --port 8080:80

# Deploy from docker-compose
synodeploy deploy docker-compose.yml

# List containers
synodeploy ps

# Remove container
synodeploy rm container-name
```

## Features

- 🚀 **One-command deployment** - Deploy containers as easily as `synodeploy run nginx`
- 🔐 **SSH key & ssh-agent support** - Works with both SSH key files and ssh-agent
- 👤 **Administrator user support** - Compatible with both `admin` and custom admin users
- 📦 **docker-compose support** - Deploy complex multi-container applications
- 🎯 **DSM 7.2+ optimized** - Built specifically for Container Manager
- 🔧 **PATH resolution** - Automatically handles Docker binary location issues
- 🧪 **Integration tested** - Verified on real Synology hardware

## Requirements

### Synology NAS
- DSM 7.2 or later
- Container Manager installed and running
- SSH access enabled with key-based authentication or ssh-agent
- User with administrator privileges and docker group membership

### Local Machine
- SSH key pair configured OR ssh-agent running
- Network access to your NAS

## Support

- 📖 [Documentation](https://github.com/scttfrdmn/synodeploy/tree/main/docs)
- 🐛 [Issue Tracker](https://github.com/scttfrdmn/synodeploy/issues)
- 💬 [Discussions](https://github.com/scttfrdmn/synodeploy/discussions)

## Automatic Updates

This formula is automatically updated via GitHub Actions and GoReleaser when new SynoDeploy releases are published. The Formula/synodeploy.rb file is generated and maintained automatically.

## License

MIT License - Copyright 2025 Scott Friedman

---

**Made with ❤️ for the Synology community**