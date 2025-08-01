# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Mintlify-powered documentation site for FlowScale AI - a no-code platform that transforms ComfyUI workflows into production-ready APIs and interactive applications. The repository contains comprehensive documentation covering getting started guides, API deployment, SDKs, and reference materials.

## Common Commands

### Development
```bash
# Start local development server
mintlify dev

# Reinstall dependencies if dev server fails
mintlify install
```

### Prerequisites
- Mintlify CLI must be installed globally: `npm i -g mintlify`
- Run commands from the root directory (where mint.json is located)

## Architecture and Structure

### Core Configuration
- **mint.json**: Main Mintlify configuration file defining navigation, theming, and site structure
- **docs.json**: Additional Mintlify schema configuration
- Uses "almond" theme with FlowScale AI branding

### Content Organization
The documentation is structured into three main tabs:

1. **Getting Started** (`/getting-started/`)
   - Overview pages (introduction, why-flowscale-ai, workflows)
   - Glossary section defining key concepts (ComfyUI, workspaces, projects, pods, models)
   - Troubleshooting guides

2. **API & Deployment** (`/deploy-api/` and `/api-reference/`)
   - Deployment guides (overview, configuration, playgrounds, scaling)
   - SDK documentation (JavaScript and Python)
   - OpenAPI specification and endpoint documentation

3. **Other References** (`/reference/`)
   - Architecture documentation (deployment models)
   - Changelog and support materials

### Content Format
- All content files use `.mdx` format (Markdown with JSX components)
- Images stored in `/images/` with organized subdirectories
- Logos and branding assets in `/logo/`
- OpenAPI specification at `/api-reference/openapi.json`

### Key Features Documented
- ComfyUI workflow deployment to REST APIs
- GPU-accelerated cloud computing (T4, L4, A100, H100)
- Team collaboration and version control
- Automatic Gradio UI generation
- Serverless scaling and cost optimization

## Content Guidelines

### FlowScale AI Context
- Platform transforms ComfyUI workflows into APIs
- Target users: AI artists, developers, agencies, researchers, startups
- Core value propositions: zero infrastructure management, seamless collaboration, production-ready APIs
- Supports file uploads, dynamic form data, and various output formats (images, videos, audio, text)

### API Authentication
- Uses `X-API-KEY` header for authentication
- All endpoints require valid API key
- Base endpoints follow `/api/v1/` pattern

### Navigation Structure
The site uses a sophisticated tab-based navigation defined in mint.json with groups and pages. When adding new content, ensure it fits within the existing information architecture.