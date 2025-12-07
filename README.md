# Yum Scaffold Templates

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A collection of project templates for the Yum Scaffold CLI tool. This repository serves as a central hub for templates that yum-scaffold pulls from dynamically.

## About

This repository contains project templates used by the [yum-scaffold](https://github.com/CodingInCarhartts/yum-scaffold) CLI tool to generate new projects. Yum-scaffold automatically discovers and lists available templates from this repository.

This repo also serves as a holding area for pull requests adding new templates to expand the available options.

## Available Templates

### nextjs-shadcn
Next.js 15 with Bun, TypeScript, Zod, Shadcn UI, and Tailwind CSS

**Tags:** nextjs, typescript, bun, shadcn, tailwind, zod

**Features:**
- Next.js 15 App Router
- TypeScript configuration
- Shadcn UI components
- Tailwind CSS for styling
- Zod for schema validation
- Bun as package manager

### python-uv
Python project with uv package manager and venv

**Tags:** python, uv, venv

**Features:**
- uv package manager
- Virtual environment setup
- Optional pytest integration
- Standard Python project structure

**Options:**
- Include pytest for testing (default: true)
- Custom Python version (default: 3.12)

### rust-cli
Rust CLI application with Tokio and Serde

**Tags:** rust, cli, tokio, serde, async

**Features:**
- Tokio async runtime
- Serde for serialization
- Optional logging with env_logger
- Cargo build system

### solidjs-bun
SolidStart with Bun, TypeScript, Tailwind, and Solid UI

**Tags:** solid, solidstart, typescript, bun, tailwind

**Features:**
- SolidStart framework
- TypeScript support
- Tailwind CSS
- Solid UI components
- Bun runtime

### sveltekit-bun
SvelteKit with Bun, Svelte 5, and TypeScript

**Tags:** svelte, sveltekit, typescript, bun

**Features:**
- SvelteKit framework
- Svelte 5
- TypeScript
- Optional Tailwind CSS
- Bun package manager

**Options:**
- Include Tailwind CSS (default: true)

### vite-ts-bun
Vite + TypeScript + Bun starter template

**Tags:** vite, typescript, bun, html

**Features:**
- Vite build tool
- TypeScript
- Optional Tailwind CSS
- Bun package manager
- Basic HTML structure

**Options:**
- Use Tailwind CSS (default: true)

## Template Structure

Each template directory contains:

- `template.toml`: Configuration file defining:
  - Metadata (name, description, version, author, tags)
  - User variables for customization
  - File mappings with Handlebars templating
  - Post-generation hooks (dependency installation, git init)

- `files/`: Directory containing template files with `.hbs` extensions for Handlebars templating

## Contributing

We welcome contributions of new templates! To add a template:

1. Create a new directory with your template name
2. Add `template.toml` configuration file
3. Create `files/` directory with your template files (use `.hbs` for templating)
4. Submit a pull request

### Guidelines
- Follow existing naming conventions
- Include comprehensive metadata in `template.toml`
- Test your template thoroughly
- Provide clear descriptions and tags
- Use Handlebars for dynamic content

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.