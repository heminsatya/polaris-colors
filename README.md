# Polaris Colors

**Version 1.5.1** · Polaris UI plugin · MIT license

A collection of configurable color palettes and color packs for styling web interfaces.

This repository contains the plugin's source and compiled distribution assets. It is maintained separately from [Polaris Core](https://github.com/sigmascript/polaris-core).

## Install

```bash
npm install polaris-colors
```

## Get started

Load the chosen compiled stylesheet in your page after any base styles whose values you want the plugin to override. The plugin provides CSS; no plugin JavaScript initialization is required. Choose only the color packs you need, rather than loading every palette by default.

Available production assets in this repository:

- `dist/css/flat.min.css`
- `dist/css/html.min.css`
- `dist/css/main.min.css`
- `dist/css/material.min.css`
- `dist/css/metro.min.css`
- `dist/css/polaris.min.css`
- `dist/css/social.min.css`

For example, use the appropriate stylesheet from `node_modules/polaris-colors/dist/css/` in your application's asset pipeline. A plain HTML project can also copy the required compiled files into its public assets.

## Development

```bash
npm install
npm run main
```

For the complete list of production and watch commands, see [Development](docs/development.md). Development dependencies remain in the plugin repository; they do not need to be deployed with a production website.

## Documentation

- [Documentation index](docs/README.md)
- [Getting started](docs/getting-started.md)
- [Development and build commands](docs/development.md)
- [Changelog](CHANGELOG.md)

## Compatibility

The current package declares `polaris-core` as a development dependency. Before publishing a future version, verify the plugin's Sass imports and compiled output against the selected Core version. Compatibility with Core 1.0.6 has **not yet been verified** in this documentation batch.

## Support and license

Report issues in the [SigmaScript repository](https://github.com/sigmascript/polaris-colors/issues) **after its transfer is completed**. Until then, use the repository's currently active issue tracker. Licensed under MIT; see `LICENSE`.
