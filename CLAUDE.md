# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Hugo-based blog site using the "loficode" theme. The project structure follows standard Hugo conventions with content stored in `matteo-blog/content/` and configuration in `matteo-blog/hugo.toml`.

## Development Commands

### Prerequisites
- Hugo static site generator must be installed

### Common Commands

```bash
# Navigate to the Hugo project directory
cd matteo-blog

# Start the development server with live reload
hugo server -D

# Build the static site
hugo

# Create a new blog post
hugo new posts/your-post-title.md

# Build with draft posts included
hugo -D
```

## Project Structure

- `matteo-blog/` - Main Hugo project directory
  - `content/posts/` - Blog posts in Markdown format
  - `public/` - Generated static site files (auto-generated, do not edit)
  - `themes/loficode/` - Custom theme directory
  - `hugo.toml` - Main configuration file
  - `archetypes/default.md` - Template for new posts

## Configuration Notes

- Site configuration is in `matteo-blog/hugo.toml`
- Profile information and social links are configured in the `[params]` section
- Navigation menu items are defined using `[[menu.main]]` entries
- The theme appears to be "loficode" based on the directory structure

## Content Management

- New posts are created in `matteo-blog/content/posts/`
- Posts use Hugo front matter (between `+++` markers) for metadata
- Default archetype sets new posts as drafts (`draft = true`)