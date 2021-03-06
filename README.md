pandoc-cookbook-template
========================

[![Pandoc test](https://github.com/Nauja/pandoc-cookbook-template/actions/workflows/pandoc-test.yml/badge.svg)](https://github.com/Nauja/pandoc-cookbook-template/actions/workflows/pandoc-test.yml)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/Nauja/pandoc-cookbook-template/master/LICENSE)

Templates for generating beautiful printable recipes from YAML metadata.

## Usage example

Generate a Just One Cookbook themed recipe from `bibimbap.yaml` example:

    pandoc \
      -o example/bibimbap.html \
      --template templates/justonecookbook/index.html \
      --css templates/justonecookbook/index.css \
      --metadata image=example/bibimbap.jpg \
      --self-contained \
      example/bibimbap.yaml

This will generate the following HTML document:

[![Bibimbap Preview](https://raw.githubusercontent.com/Nauja/pandoc-cookbook-template/master/example/bibimbap-justonecookbook-preview.jpg)](https://raw.githubusercontent.com/Nauja/pandoc-cookbook-template/master/example/bibimbap-justonecookbook-preview.jpg)

Alternatively, if you want the Cuisine AZ template:

    pandoc \
      -o example/bibimbap.html \
      --template templates/cuisineaz/index.html \
      --css templates/cuisineaz/index.css \
      --metadata image=example/bibimbap.jpg \
      --self-contained \
      example/bibimbap.yaml

This will generate the following HTML document:

[![Bibimbap Preview](https://raw.githubusercontent.com/Nauja/pandoc-cookbook-template/master/example/bibimbap-cuisineaz-preview.jpg)](https://raw.githubusercontent.com/Nauja/pandoc-cookbook-template/master/example/bibimbap-cuisineaz-preview.jpg)

You can generate `sandbox.yaml` - a recipe used to showcase all things you can write and some specific cases - the same way:

    pandoc \
      -o example/sandbox.html \
      --template templates/<template>/index.html \
      --css templates/<template>/index.css \
      --self-contained \
      example/sandbox.yaml

## License

Licensed under the [MIT](LICENSE) License.
