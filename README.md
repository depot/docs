# Depot Documentation

This repository contains the official documentation for [Depot](https://depot.dev/docs), a build acceleration platform that makes development workflows exponentially faster.

## About Depot

Depot is a build acceleration platform that provides:
- **Remote container builds** - Up to 40x faster Docker builds with native multi-platform support
- **Global container registry** - High-performance, globally-distributed container registry with CDN-backed delivery
- **GitHub Actions Runners** - Up to 3x faster runners with 30% faster CPUs and 10x faster networking
- **Universal build cache** - Remote caching for Bazel, Go, Gradle, Turborepo, sccache, and Pants
- **Build API** - Programmatic access to container build infrastructure

## Repository Structure

```
content/
├── agents/              # AI agent documentation
│   ├── claude-code/     # Claude Code integration guides
│   └── overview.mdx     # General agent overview
├── cache/               # Universal build cache documentation
│   ├── authentication.mdx
│   ├── overview.mdx
│   └── reference/       # Tool-specific cache guides (Bazel, Gradle, etc.)
├── cli/                 # Depot CLI documentation
│   ├── authentication.mdx
│   ├── installation.mdx
│   └── reference.mdx
├── container-builds/    # Remote container builds documentation
│   ├── how-to-guides/   # Implementation guides and best practices
│   ├── overview.mdx
│   ├── quickstart.mdx
│   ├── reference/       # CI/CD platform integrations
│   └── troubleshooting.mdx
├── github-actions/      # GitHub Actions runners documentation
│   ├── overview.mdx
│   ├── quickstart.mdx
│   ├── reference/       # Integration guides
│   └── runner-types.mdx
├── integrations/        # Third-party integrations
├── managed/             # Depot managed services (AWS, GPUs)
├── overview/            # Platform overview and concepts
│   ├── core-concepts.mdx
│   ├── faq.mdx
│   ├── index.mdx
│   └── security.mdx
└── registry/            # Container registry documentation
    ├── overview.mdx
    └── quickstart.mdx
```

## Development

This documentation site uses:
- **Package Manager**: pnpm
- **Formatting**: Prettier with custom configuration
- **Content Format**: MDX files with frontmatter

### Available Scripts

```bash
pnpm fmt        # Format all files
pnpm fmt:check  # Check formatting
```

## Documentation Structure

The documentation is organized into major product areas:

1. **Overview** - Introduction, core concepts, FAQ, and security information
2. **Container Builds** - Remote Docker builds with comprehensive guides and CI integrations
3. **GitHub Actions** - Accelerated runners with quickstart and reference materials
4. **Cache** - Universal build cache for multiple development tools
5. **Registry** - Global container registry documentation
6. **CLI** - Command-line interface guides and reference
7. **Agents** - AI agent integrations and usage guides
8. **Integrations** - Third-party tool integrations
9. **Managed** - Enterprise and managed service options

Each section includes quickstart guides, detailed how-to documentation, and comprehensive reference materials for different platforms and use cases.

## Contributing

When contributing to the documentation:
1. Follow the existing MDX structure and frontmatter format
2. Run `pnpm fmt` before committing to ensure consistent formatting
3. Test your changes locally before submitting

For more information, visit [depot.dev/docs](https://depot.dev/docs).
