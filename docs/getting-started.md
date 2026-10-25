# Getting started

## Install

```bash
npm install polaris-colors
```

## Distribution files

- `dist/css/flat.min.css`
- `dist/css/html.min.css`
- `dist/css/main.min.css`
- `dist/css/material.min.css`
- `dist/css/metro.min.css`
- `dist/css/polaris.min.css`
- `dist/css/social.min.css`

## Integration

Load the chosen compiled stylesheet in your page after any base styles whose values you want the plugin to override. The plugin provides CSS; no plugin JavaScript initialization is required. Choose only the color packs you need, rather than loading every palette by default.

When using a package manager, import or copy the appropriate compiled asset from `node_modules/polaris-colors/dist/`. Keep source Sass files available when customizing the plugin.

## Important distinctions

- `src/` contains development source.
- `dist/` contains compiled assets intended for consumption.
- `index.js` is not documented here as a browser UI initialization API.
- Existing public CSS names and, where applicable, JavaScript APIs should remain stable during maintenance.
