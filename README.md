# Eladio Rocha — Retro Portfolio

A **static personal portfolio with a retro desktop aesthetic**, built with HTML, Bootstrap styles, and pixel-art assets. It presents an introduction, technical skills, selected projects, and contact links on a single page.

## Featured content

- Introduction, career interests, and hobbies.
- Pixel-art icons for React, Node.js, MongoDB, Python, MySQL, and Git.
- Project cards for Motum, Trading Quiz, and Bob the Reporter.
- Email, GitHub, and LinkedIn contact links.

The page is a snapshot of the portfolio content stored in this repository; project descriptions and external profiles may need updating over time.

## View locally

No package manager or build process is required. With Python 3 installed:

```sh
git clone https://github.com/EladioRocha/portfolio.git
cd portfolio
python -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000` in a browser. Stop the server with `Ctrl+C`.

The page uses local styles, fonts, images, and Bootstrap JavaScript. jQuery is loaded from a CDN, so navigation behavior that depends on it needs an internet connection.

## Customize the portfolio

1. Edit [index.html](index.html) to update the introduction, skills, project descriptions, and contact destinations.
2. Replace project thumbnails in [assets/images/portfolio](assets/images/portfolio) and update their corresponding image paths.
3. Keep navigation targets aligned with the page sections: `home`, `skills`, `portfolio`, and `contact`.
4. Update the inline styles in `index.html` for page-specific colors and spacing. The Bootstrap files provide the underlying theme.

## Project structure

| Path | Purpose |
| --- | --- |
| [index.html](index.html) | Page content, section links, and inline styling. |
| [assets/css](assets/css) | Bootstrap theme, styles, and pixel font files. |
| [assets/fonts](assets/fonts) | Glyphicon font files. |
| [assets/images](assets/images) | Skill icons, contact icons, and project thumbnails. |
| [assets/js](assets/js) | Bundled Bootstrap scripts. |

## Publishing and verification

The repository can be served by a static host with `index.html` at the site root and the `assets` directory alongside it. No backend or environment variables are required. This guide does not assume an active deployment URL.

There is no automated test suite. Before publishing changes, check the page at desktop and mobile widths, expand the mobile menu, verify images and section links, and review the external project and contact destinations. Preserve third-party notices in the bundled Bootstrap assets.
