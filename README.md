# Depot Documentation

This repository contains the official documentation for [Depot](https://depot.dev/docs), a comprehensive build acceleration platform that makes development workflows exponentially faster.

## About Depot

Depot is a build acceleration platform designed to solve the performance bottlenecks in modern development workflows. The platform provides:

- **Remote container builds** - Up to 40x faster Docker builds with native multi-platform support, persistent layer caching, and high-performance compute
- **Global container registry** - High-performance, globally-distributed container registry with CDN-backed delivery and seamless integration
- **GitHub Actions Runners** - Up to 3x faster runners with 30% faster CPUs, 10x faster networking, and optimized environments
- **Universal build cache** - Remote caching infrastructure for Bazel, Go, Gradle, Turborepo, sccache, Pants, and more
- **Build API** - Programmatic access to container build infrastructure for custom integrations
- **AI Agent Integration** - Native support for Claude Code and other AI development tools

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

## Technical Overview

### Project Structure

This is a documentation repository built with:

- **Content Format**: MDX files with YAML frontmatter for metadata
- **Package Manager**: pnpm (v9.5.0+)
- **Code Formatting**: Prettier with custom configuration
- **File Organization**: Hierarchical content structure mirroring product features

### Content Architecture

All documentation content is stored in the `content/` directory, organized by product area:

- Each section contains overview, quickstart, and reference materials
- MDX files support React components and rich formatting
- Frontmatter includes title, description, and SEO metadata

### Development Workflow

#### Prerequisites

- Node.js (compatible with pnpm v9.5.0)
- pnpm package manager

#### Available Scripts

```bash
pnpm fmt        # Format all files using Prettier
pnpm fmt:check  # Check formatting without making changes
```

#### Development Best Practices

- Run `pnpm fmt` before committing to ensure consistent code style
- Follow the existing MDX structure and frontmatter format
- Test documentation changes locally before submitting
- Maintain the hierarchical organization of content sections

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

### Getting Started

1. Clone the repository and install dependencies with `pnpm install`
2. Make your documentation changes in the appropriate `content/` subdirectory
3. Follow the existing MDX structure and frontmatter format
4. Run `pnpm fmt` to ensure consistent formatting
5. Test your changes locally before submitting

### Content Guidelines

- **Structure**: Maintain the established content hierarchy and naming conventions
- **Formatting**: Use MDX syntax with appropriate frontmatter metadata
- **Style**: Follow the existing tone and technical writing standards
- **Components**: Leverage existing React components when available
- **Cross-references**: Use relative links within the documentation

### File Organization

- Place new content in the appropriate product section under `content/`
- Use descriptive filenames that match the content structure
- Include proper frontmatter with title, description, and ogTitle fields
- Follow the existing pattern of overview → quickstart → reference → how-to-guides

For more information about Depot's features and capabilities, visit [depot.dev/docs](https://depot.dev/docs).
