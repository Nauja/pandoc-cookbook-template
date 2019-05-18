pandoc-justonecookbook-template
===============================

[![Build Status](https://travis-ci.org/Nauja/pandoc-justonecookbook-template.png?branch=master)](https://travis-ci.org/Nauja/pandoc-justonecookbook-template)

Template for generating Just One Cookbook themed printable recipes from YAML metadata.

### Usage example

Generate a self-contained HTML document from `melon-pan.yaml` example recipe:

    pandoc \
      -o example/melon-pan.html \
      --template template.html \
      --css template.css \
      --metadata image=example/melon-pan.jpg \
      --self-contained \
      example/melon-pan.yaml
