# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a VitePress-based blog about Korean radio streaming apps ("KoreaRadioBlog"). VitePress is a Vue.js-powered static site generator optimized for technical documentation and blogs.

## Architecture

- **VitePress**: Static site generator using Vue.js and Vite
- **Configuration**: `.vitepress/config.mts` contains site configuration including navigation, sidebar, and theme settings
- **Content**: Markdown files in the root directory serve as pages
- **Home Page**: `index.md` with hero section and feature highlights
- **Build Output**: Generated to `.vitepress/dist/`

## Development Commands

```bash
# Start development server with hot reload
npm run docs:dev

# Build static site for production
npm run docs:build

# Preview built site locally
npm run docs:preview
```

## Content Structure

- `index.md`: Home page with hero section and features
- `markdown-examples.md`: Demonstrates VitePress markdown extensions
- `api-examples.md`: Shows VitePress runtime API usage
- `.vitepress/config.mts`: Site configuration and theme settings

## VitePress Features

- Supports Vue components in markdown
- Built-in syntax highlighting via Shiki
- Custom containers (info, tip, warning, danger, details)
- Runtime APIs via `useData()` hook
- Automatic sidebar and navigation generation

## File Conventions

- Use `.md` for content pages
- Configuration uses TypeScript (`.mts`)
- Static assets go in `.vitepress/public/` (if needed)
- Custom components in `.vitepress/theme/` or `.vitepress/components/`