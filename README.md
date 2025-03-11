[![theme badge](https://img.shields.io/badge/ELIXIR%20toolkit%20theme-jekyll-blue?color=0d6efd)](https://github.com/ELIXIR-Belgium/elixir-toolkit-theme)

# mTeSS-X

This repository serves the [project website for mTeSS-X](https://elixirtess.github.io/mTeSS-X/). It uses the [ELIXIR Toolkit Theme](https://elixir-belgium.github.io/elixir-toolkit-theme/). 

## Design

This site follows the [OSCARS comms kit](https://www.oscars-project.eu/sites/default/files/2024-12/OSCARS-FundedProjects-CommsKit.pdf).

## Relative vs. absolute paths

There are a few assets which are loaded using an absolute path. 
These work correctly when viewing the site through GitHub Pages as intended (with `/mTeSS-X/` at the root). 
They do not work correctly when running the site locally with Jekyll. It must be possible to correct this with the Liquid `relative_url` function.

- `_data/footer.yml`:
  - `/mTeSS-X/images/CreativeCommon_88x31.png`
- `_sass/_custom_classes.scss`:
  - `/mTeSS-X/assets/fonts/PlusJakartaSans-VariableFont_wght.woff`
  - `/mTeSS-X/assets/fonts/PlusJakartaSans-Italic-VariableFont_wght.woff`

Note, these fonts are served with the site directly, not from the Google Fonts service, to avoid additional tracking. 