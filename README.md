# hugo-shortcodes

[![Awesome](https://awesome.re/badge.svg)](https://github.com/budparr/awesome-hugo)

## About


It is a [Hugo](https://gohugo.io) theme component providing a shortcodes





## Usage

1. Add the `hugo-shortcodes` as a submodule to be able to get upstream changes later 

`git submodule add https://github.com/talz26/hugo-shortcodes.git themes/hugo-shortcodes`

2. Add `hugo-shortcodes` as the left-most element of the `theme` list variable in your site's or theme's configuration file `config.yaml` or `config.toml`. Example, with `config.yaml`:
    ```yaml

    theme: ["hugo-shortcodes", "my-theme"]
    ```
    or, with `config.toml`,

    ```toml
    theme = ["hugo-shortcodes, "my-theme"]

