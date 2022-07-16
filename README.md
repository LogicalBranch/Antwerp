# Antwerp
## Description:
Build program for [logicalbranch.github.io](https://logicalbranch.github.io) ported from [Node.js](https://nodejs.org/en/) and [Pug](https://pugjs.org/api/getting-started.html) to [Rust](https://www.rust-lang.org/) & [Tera](https://tera.netlify.app/) and is in the process of being converted into a minimalist standalone framework for generating static websites.

## About:
This program takes given resources and copies (static files), compiles (SCSS stylesheets), and renders (Tera templates) to generate a static website in a `./dist` folder.

It was ported from Node.js & Pug to Rust & Tera to improve the performance and speed of the build program, resulting in an (optimised) binary where the real (total elapsed) build time is - on average - 97.50% faster than its Node.js counterpart, a decrease in average build speed from 2.8 seconds to 0.07 seconds.

## Todo:
- [x] Document existing code
- [x] Remove unnecessary `lib.rs` methods
- [x] Allow for user defined directory structures
- [ ] Add (opt-in) support for [SWC](https://swc.rs/)
- [ ] Standardise and integrate the `Article` module into Antwerp


## Ideas:
- [ ] Implement a config file (`Antwerp.toml`)
  - [ ] Only print if `verbose` is enabled
  - [ ] Move `empty_root` to a config file
    - [ ] confirm delete if option is true (?)
- [ ] Implement CLI interface
  - [ ] Call init methods for config options
  - [ ] Implement a `watch` CLI option (`--watch`)
  - [ ] Generate new projects
    - [ ] Generate directory structure
    - [ ] Generate sample files and source code

## Notes:
  * Scopes for `print` calls in `core.rs` are placeholders

## Useful links:
 * https://programming-idioms.org/cheatsheet/Rust
 * https://github.com/connorskees/grass/issues/19
 * https://stackoverflow.com/a/29008355/10415695