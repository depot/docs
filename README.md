# Depot Docs

This repository contains the documentation for Depot, a platform for faster Docker container builds and intelligent caching. The documentation is hosted at [depot.dev/docs](https://depot.dev/docs).

## Repository Structure

The documentation is organized into the following main sections:

### `/content/`

The main documentation content organized by feature area:

- **`agents/`** - Documentation for Depot's AI agents, including Claude Code integration
- **`cache/`** - Build caching documentation with support for various tools (Bazel, Go, Gradle, Maven, Turbo, etc.)
- **`cli/`** - Command-line interface documentation including installation, authentication, and reference
- **`container-builds/`** - Core container building features including:
  - How-to guides for Docker builds, ARM containers, CI/CD integration
  - Optimal Dockerfile examples for Node.js, Python, Rust
  - Private registry configuration
  - Troubleshooting guides
- **`github-actions/`** - GitHub Actions integration and runner types
- **`integrations/`** - Third-party integrations (Tailscale, etc.)
- **`managed/`** - Managed infrastructure options including AWS deployment and GPU usage
- **`overview/`** - Core concepts, FAQ, security documentation
- **`registry/`** - Container registry functionality

### Development

- **`package.json`** - Project configuration with Prettier formatting
- **`pnpm-lock.yaml`** - Package manager lock file

The documentation uses MDX format and is structured to provide comprehensive coverage of Depot's container building, caching, and CI/CD integration capabilities.
