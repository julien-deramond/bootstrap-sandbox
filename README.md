# Bootstrap Sandbox

A sandbox Bootstrap-based library for testing and experimenting with future Bootstrap implementations.

## Usage

This library is intended to be used in place of the Bootstrap library for testing and experimenting with future Bootstrap implementations. It is not intended to be used in production.

In order to be clear about the purpose of this library, released files have been renamed to include the `-sandbox` suffix. This is to prevent confusion with the official Bootstrap library.

CSS files:

| CSS File | Minified CSS File | RTL CSS File | Minified RTL CSS File |
| --- | --- | --- | --- |
| `bootstrap-sandbox.css` | `bootstrap-sandbox.min.css` | `bootstrap-sandbox.rtl.css` | `bootstrap-sandbox.rtl.min.css` |
| `bootstrap-sandbox-grid.css` | `bootstrap-sandbox-grid.min.css` | `bootstrap-sandbox-grid.rtl.css` | `bootstrap-sandbox-grid.rtl.min.css` |
| `bootstrap-sandbox-reboot.css` | `bootstrap-sandbox-reboot.min.css` | `bootstrap-sandbox-reboot.rtl.css` | `bootstrap-sandbox-reboot.rtl.min.css` |
| `bootstrap-sandbox-utilities.css` | `bootstrap-sandbox-utilities.min.css` | `bootstrap-sandbox-utilities.rtl.css` | `bootstrap-sandbox-utilities.rtl.min.css` |

JS files:

| JS File | Minified JS File |
| --- | --- |
| `bootstrap-sandbox.js` | `bootstrap-sandbox.min.js` |
| `bootstrap-sandbox.bundle.js` | `bootstrap-sandbox.bundle.min.js` |
| `bootstrap-sandbox.esm.js` | `bootstrap-sandbox.esm.min.js` |

## Discrepancies with Bootstrap

- No `dist` or `js/dist` folders are stored in the repository. Instead, they are generated locally when running the `npm run dist` command.
  - ```diff
    -"js-lint": "eslint --cache --cache-location .cache/.eslintcache --report-unused-disable-directives --ext .html,.js,.mjs,.md .",
    +"js-lint": "npm run dist && eslint --cache --cache-location .cache/.eslintcache --report-unused-disable-directives --ext .html,.js,.mjs,.md .",
    ``` 
- [Storybook](https://storybook.js.org/) is used to showcase components to make it easier to test and experiment with future Bootstrap implementations.
  - Simply run `npm run storybook` locally to start the Storybook server.
 
  - <details>
    <summary>Commits</summary>

    - https://github.com/julien-deramond/bootstrap-sandbox/commit/d7671eceb3efe2991c2afa198b1642a082004c8e
  </details>

## Sponsors

<p align="center">
  <a href="https://cdn.jsdelivr.net/gh/julien-deramond/static/sponsors.svg">
    <img src='https://cdn.jsdelivr.net/gh/julien-deramond/static/sponsors.svg'/>
  </a>
</p>

## License

[MIT](LICENSE)
