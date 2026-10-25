# Development

## Prerequisites

Install Node.js and the package's development dependencies:

```bash
npm install
```

The current project scripts are:

| Script | Command |
|---|---|
| `npm run main` | `sass src/scss/main.scss dist/css/main.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run main-dev` | `sass src/scss/main.scss dist/css/main.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run polaris` | `sass src/scss/polaris.scss dist/css/polaris.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run polaris-dev` | `sass src/scss/polaris.scss dist/css/polaris.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run material` | `sass src/scss/material.scss dist/css/material.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run material-dev` | `sass src/scss/material.scss dist/css/material.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run html` | `sass src/scss/html.scss dist/css/html.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run html-dev` | `sass src/scss/html.scss dist/css/html.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run flat` | `sass src/scss/flat.scss dist/css/flat.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run flat-dev` | `sass src/scss/flat.scss dist/css/flat.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run metro` | `sass src/scss/metro.scss dist/css/metro.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run metro-dev` | `sass src/scss/metro.scss dist/css/metro.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |
| `npm run social` | `sass src/scss/social.scss dist/css/social.min.css --style compressed --load-path=node_modules --no-source-map --silence-deprecation=import,global-builtin,if-function` |
| `npm run social-dev` | `sass src/scss/social.scss dist/css/social.css --watch --load-path=node_modules --silence-deprecation=import,global-builtin,if-function` |

## Production and watch commands

One-shot commands: `npm run main`, `npm run polaris`, `npm run material`, `npm run html`, `npm run flat`, `npm run metro`, `npm run social`.

Watch commands: `npm run main-dev`, `npm run polaris-dev`, `npm run material-dev`, `npm run html-dev`, `npm run flat-dev`, `npm run metro-dev`, `npm run social-dev`. Watchers continue running until stopped with `Ctrl+C`.

## Release checks

1. Run `npm audit` and inspect any reported advisories.
2. Run all applicable one-shot build commands.
3. Check watch commands individually, then stop each with `Ctrl+C`.
4. Review `git diff --stat`, `git diff --check`, and generated `dist/` changes.
5. Run `npm pack --dry-run` to inspect published contents.
6. Verify compatibility with the intended Polaris Core version before selecting a new release version.

The current `npm test` script is a placeholder, not a test suite; do not treat it as a passing test. Avoid changing public class names, Sass customization names, or JavaScript interfaces without a compatibility review.
