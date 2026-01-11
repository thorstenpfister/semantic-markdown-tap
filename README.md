# Homebrew Tap for Semantic Markdown

This is the official Homebrew tap for [semantic-markdown](https://github.com/thorstenpfister/semantic-markdown), a Go library and CLI tool for converting HTML to clean, semantic Markdown optimized for Large Language Models (LLMs).

## Installation

### Tap and Install

```bash
# Add this tap to your Homebrew
brew tap thorstenpfister/semantic-markdown-tap

# Install semantic-md
brew install semantic-md
```

### Direct Install

You can also install directly without explicitly tapping:

```bash
brew install thorstenpfister/semantic-markdown-tap/semantic-md
```

## Available Formulae

### semantic-md

Convert HTML to clean, semantic Markdown optimized for LLMs.

**Features:**
- Main content detection - Automatically extracts primary content
- Metadata extraction - Captures Open Graph, Twitter Cards, and JSON-LD
- URL refification - Converts long URLs to short references
- Table support - Full support for complex tables
- Smart escaping - CommonMark-compliant context-aware escaping
- Semantic HTML - Preserves semantic meaning from HTML5 elements

**Usage:**

```bash
# Convert HTML file to Markdown
semantic-md convert -i input.html -o output.md

# Extract main content only
semantic-md convert -i page.html -o content.md --extract-main

# Include metadata and refify URLs
semantic-md convert -i page.html -o output.md -m extended -r

# Fetch from URL and convert
curl -s https://example.com | semantic-md convert > output.md
```

**Project Homepage:** https://github.com/thorstenpfister/semantic-markdown

## Updating

To update to the latest version:

```bash
brew update
brew upgrade semantic-md
```

## Supported Platforms

- macOS (Intel and Apple Silicon)
- Linux (x86_64 and ARM64)

## Issues and Support

- Report issues: https://github.com/thorstenpfister/semantic-markdown/issues
- View releases: https://github.com/thorstenpfister/semantic-markdown/releases
- Documentation: https://github.com/thorstenpfister/semantic-markdown

## About Homebrew Taps

Homebrew taps are third-party repositories that extend Homebrew's capabilities. This tap provides easy installation and updates for semantic-markdown tools.

Learn more about taps: https://docs.brew.sh/Taps
