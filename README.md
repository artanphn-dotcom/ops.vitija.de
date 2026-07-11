# ops.vitija.de

Static operations reference portal for network, security, Linux, cloud, and GitHub command lookups.

## Overview

This project is a plain HTML, CSS, and JavaScript site built as a fast lookup hub for operational CLI commands. The landing page links to vendor-specific reference pages and a network utilities console. Each reference page is self-contained and designed for quick use during troubleshooting, change windows, or incident response.

There is no build step, framework, or backend. The site can be opened directly in a browser or served from any static web host.

## What is included

- A landing page in `index.html`
- A network utilities console in `network-tools.html`
- Searchable command-reference pages for:
	- Cisco
	- Arista
	- Fortinet
	- Palo Alto Networks
	- Juniper
	- Check Point
	- SonicWall
	- Barracuda Networks
	- F5
	- Linux
	- AWS
	- GitHub
- Shared site icon in `favicon.svg`

## Key features

- Static single-file reference pages
- Client-side search and filtering
- Click-to-copy command buttons
- Responsive layout for desktop and mobile use
- No runtime dependencies or application server required
- Easy deployment to any static hosting platform

## Project structure

```text
.
|-- index.html
|-- network-tools.html
|-- cisco-cli-reference.html
|-- arista-cli-reference.html
|-- fortigate-cli-reference.html
|-- paloalto-cli-reference.html
|-- juniper-cli-reference.html
|-- checkpoint-cli-reference.html
|-- sonicwall-cli-reference.html
|-- barracuda-cli-reference.html
|-- f5-cli-reference.html
|-- linux-cli-reference.html
|-- aws-cli-reference.html
|-- github-cli-reference.html
|-- favicon.svg
`-- README.md
```

## Local usage

### Option 1: Open directly

Open `index.html` in a browser.

### Option 2: Serve locally

Using Python:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Deployment

Because the site is fully static, it can be deployed as-is to platforms such as:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- Any standard web server serving static files

Set `index.html` as the default entry point.

## Editing and extending

To add or update a reference page:

1. Duplicate an existing `*-cli-reference.html` file that matches the layout you want.
2. Update the page title, hero text, and command dataset in that file.
3. Add or update the corresponding card in `index.html`.
4. Verify the page is linked correctly from the main menu.

The current reference pages embed their data directly in JavaScript, which makes the site simple to maintain and easy to host anywhere.

## Notes

- The site is static and works without a backend.
- Some pages load Google Fonts from `fonts.googleapis.com` and `fonts.gstatic.com`. If those requests are blocked, the site still renders using fallback fonts.
- `index.html` currently links to `gcp-cli-reference.html`, but that file is not present in this repository.

## Intended use

This repository is useful for:

- Network engineers
- Systems administrators
- Security engineers
- SRE and operations teams
- Anyone who wants a lightweight internal command-reference portal
