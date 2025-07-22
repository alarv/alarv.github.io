# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is "Geras" - a web-based JavaScript game about aging. It's a GitHub Pages hosted website (alarv.github.io) that runs entirely in the browser. The game appears to be built with vanilla JavaScript and uses HTML5 Canvas for rendering.

## Project Structure

- `index.html` - Root redirect page that forwards visitors to `/geras/`
- `geras/` - Main game directory containing:
  - `index.html` - Main game HTML file with game container, Google Analytics, and GitHub corner link
  - `game.js` - Main game logic (compiled/minified JavaScript bundle)
  - `game.js.map` - Source map for debugging
  - `style.css` - Styling for the webpage including animated cloud background
  - `assets/` - Game assets (sprites, backgrounds, icons)
  - `favicon.ico` - Site favicon

## Development

This is a static website project. The main game logic is contained in a compiled JavaScript bundle (`game.js`) which appears to be built from a larger codebase, likely using a build tool like webpack or similar.

### Key Technologies
- Vanilla JavaScript (compiled bundle)
- HTML5 Canvas for game rendering
- CSS animations for background effects
- Google Analytics for tracking

### Game Architecture
Based on code analysis, the game uses:
- Animation system with sprite management
- Event-driven architecture with EventEmitter
- Object pooling and class-based architecture
- Geometry utilities (circles, points, rectangles)
- Alpha blending and rendering pipeline

### Deployment
This is deployed to GitHub Pages as a static site. The game is accessible at `alarv.github.io/geras/` with the root domain redirecting to the game directory.

## Important Notes

The main game logic is in a minified bundle, so direct code modifications should be made to the source files (not included in this repository). This repository appears to be the built/compiled output for GitHub Pages hosting.