# Agent Guidelines for inkdrop-catppuccin-mocha-syntax

## Project Overview
Inkdrop syntax theme package implementing Catppuccin Mocha color scheme using CSS.

## Build Commands
- Build: `npm run build` (compiles LESS to CSS - NOTE: styles/less/default.less source file appears missing)
- No tests or linting configured

## Code Style

### CSS/Styling
- Use CSS custom properties (variables) with `--ctp-` prefix for Catppuccin colors
- Follow existing color mapping: keywords=mauve, strings=green, numbers=peach, functions=blue, comments=overlay0
- Scope all styles under `.editor .CodeMirror` selectors
- Use nested CSS syntax for related selectors
- Apply `!important` sparingly, only when overriding specificity issues
- Color comments should be italic with `font-style: italic`

### Naming Conventions
- CSS classes follow CodeMirror's naming: `.cm-{token-type}` (e.g., `.cm-keyword`, `.cm-string`)
- Color variables: `--ctp-{color-name}` matching Catppuccin palette

### File Organization
- Main CSS output: `styles/catppuccin-mocha.css`
- Version in package.json should follow semver
