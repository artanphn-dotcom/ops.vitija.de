# ops.vitija.de

A lightweight, static command-reference portal for network, security, Linux, cloud, and developer operations.

[![Static Site](https://img.shields.io/badge/site-static-0f172a?style=flat-square&logo=html5&logoColor=white)](#)
[![HTML5](https://img.shields.io/badge/HTML-5-E34F26?style=flat-square&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS-3-1572B6?style=flat-square&logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![No Backend](https://img.shields.io/badge/backend-none-22c55e?style=flat-square)](#)

---

## Overview

ops.vitija.de is a self-contained reference website designed for fast command lookup during troubleshooting, maintenance windows, and incident response. It provides vendor-specific CLI references and a small utilities section in a format that is easy to browse, easy to deploy, and easy to maintain.

The project is intentionally simple: no framework, no build step, and no backend are required. The site runs entirely in the browser and can be served from any static host.

## Visual Guide

A visual overview of the project structure and purpose is included in the repository:

<p align="center">
  <img src="studyguide.png" alt="ops.vitija.de visual study guide" width="1200">
</p>

## Included References

### Network and Security

- Cisco
- Arista
- Fortinet
- Palo Alto Networks
- Juniper
- Check Point
- SonicWall
- Barracuda Networks
- F5

### Systems, Cloud, and Development

- Linux
- AWS
- GitHub

### Utilities

- Network tools console
- Main portal landing page

## Key Features

- Fast browsing of operational command references
- Client-side search and filtering
- Copy-to-clipboard support for commands
- Responsive layout for desktop and mobile use
- Zero dependency installation or build process
- Easy deployment to static hosting platforms

## Project Structure

```text
.
├── index.html
├── network-tools.html
├── arista-cli-reference.html
├── aws-cli-reference.html
├── barracuda-cli-reference.html
├── checkpoint-cli-reference.html
├── cisco-cli-reference.html
├── f5-cli-reference.html
├── fortigate-cli-reference.html
├── github-cli-reference.html
├── juniper-cli-reference.html
├── linux-cli-reference.html
├── paloalto-cli-reference.html
├── sonicwall-cli-reference.html
├── favicon.svg
├── studyguide.png
└── README.md
```

## Usage

### Open Locally

You can view the site by opening [index.html](index.html) directly in a browser.

### Run a Local Web Server

If you prefer a local HTTP server, use:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment

This project can be deployed as-is to any static hosting service, including:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- Nginx
- Apache

Upload the repository contents and serve the site from the root directory.

## Customization

To add a new reference page:

1. Create a new HTML reference file based on an existing one.
2. Update the page content and embedded command data.
3. Add the new entry to the main landing page.
4. Verify navigation and copy functionality.

## Notes

- The site relies on standard browser capabilities and does not require a database or backend service.
- Some pages may load external fonts; if those requests are blocked, the page will still render with fallback styling.
- Commands and procedures should always be reviewed for accuracy and appropriateness within your environment before use.

## License

This repository is intended for operational and internal use. If you plan to distribute it publicly, please confirm that the included content aligns with your organization’s documentation and security policies.
