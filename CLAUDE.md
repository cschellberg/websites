# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project purpose

This repository hosts multiple independent static HTML websites (see `spec.md`). There is no shared build system, framework, or server-side code — sites are plain HTML/CSS/images served as static files.

## Structure

- Each subdirectory at the repo root is one self-contained site.
- A site's subdirectory contains everything for that site: its HTML pages, CSS files, and images.
- images should be in the same directory not a separate subdirectory. CSS files should also be in the same directory as the HTML files.
- CSS files are linked from HTML files within the same subdirectory; images are referenced the same way. Do not share assets across site subdirectories — each site is standalone, with no shared assets or dependencies between sites.

## Content and design requirements

- All site content must be written in Spanish.
- All sites must be designed responsively and be mobile-friendly.

## Working in this repo

- When adding a new site, create a new top-level subdirectory for it rather than adding pages into an existing site's directory.
- There is no build, lint, or test tooling in this repo currently — sites are static files that can be opened/served directly.
