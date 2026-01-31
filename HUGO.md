# Hugo Site Setup

This site is configured to use [Hugo](https://gohugo.io/) for static site generation with the [Congo theme](https://github.com/jpanther/congo).

## Requirements

- Hugo Extended v0.142.0 or later
- Git (for managing the theme submodule)

## Installation

1. Clone the repository with submodules:
   ```bash
   git clone --recurse-submodules https://github.com/lichterberci/lichterberci.github.io.git
   cd lichterberci.github.io
   ```

2. If you've already cloned the repository, initialize the submodule:
   ```bash
   git submodule update --init --recursive
   ```

## Building the Site

To build the site:
```bash
hugo
```

The generated site will be in the `public/` directory.

## Local Development

To run a local development server with live reload:
```bash
hugo server
```

Then visit http://localhost:1313/ in your browser.

## Adding Content

Create new content using:
```bash
hugo new content/posts/my-post.md
```

## Theme Configuration

The site uses the Congo theme with some modifications. See `themes/congo/MODIFICATIONS.md` for details on the changes made to ensure compatibility.

### Key Configuration Files

- `config/_default/hugo.toml` - Main Hugo configuration
- `config/_default/languages.hu.toml` - Hungarian language settings
- `config/_default/params.toml` - Theme parameters
- `config/_default/markup.toml` - Markdown rendering options

## Updating the Theme

To update the Congo theme:
```bash
git submodule update --remote themes/congo
```

Note: After updating, you may need to re-apply the modifications documented in `themes/congo/MODIFICATIONS.md`.

## Deployment

The site is configured for deployment to GitHub Pages at https://lichterberci.github.io/

For more information about Congo theme features and configuration options, visit the [Congo documentation](https://jpanther.github.io/congo/docs/).
