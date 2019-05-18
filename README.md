pandoc-justonecookbook-template
===============================

[![Build Status](https://travis-ci.org/Nauja/pandoc-justonecookbook-template.png?branch=master)](https://travis-ci.org/Nauja/pandoc-justonecookbook-template)

Template for generating Just One Cookbook themed printable recipes from YAML metadata.

### Usage example

Generate a self-contained HTML document from `bibimbap.yaml` example recipe:

    pandoc \
      -o example/bibimbap.html \
      --template template.html \
      --css template.css \
      --metadata image=example/bibimbap.jpg \
      --self-contained \
      example/bibimbap.yaml

This will generate the following HTML document:

[![Bibimbap Preview](https://raw.githubusercontent.com/Nauja/pandoc-justonecookbook-template/master/example/bibimbap-preview.jpg)](https://raw.githubusercontent.com/Nauja/pandoc-justonecookbook-template/master/example/bibimbap-preview.jpg)

You can generate `sandbox.yaml` - a recipe used to showcase all things you can write and some specific cases - the same way:

    pandoc \
      -o example/sandbox.html \
      --template template.html \
      --css template.css \
      --self-contained \
      example/sandbox.yaml
