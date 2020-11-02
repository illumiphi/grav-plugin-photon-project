<a href="https://photon-platform.net/">
    <img src="https://photon-platform.net/user/images/photon-logo-banner.png" alt="photon" title="photon" align="right" height="120" />
</a>


# photon ✴ Project

## 0.1.0

---


> project templates and styles

- [configuration](#configuration)
- [templates](#templates)
- [scaffolds](#scaffolds)
- [scss](#scss)
- [assets](#assets)
- [languages](#languages)

# configuration
blueprints.yaml

fields:
- enabled
- built_in_css
- built_in_js

Before configuring this plugin, you should copy the `user/plugins/photon-project/photon-project.yaml` to `user/config/plugins/photon-project.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```yaml
enabled: true
built_in_css: true
built_in_js: true

description: Custom Text added by the **photon-project** plugin (disable plugin to remove)
```

Note that if you use the admin plugin, a file with your configuration, and named photon-project.yaml will be saved in the `user/config/plugins/` folder once the configuration is saved in the admin.


# blueprints

```sh
blueprints
└── project.yaml
```

### Project
project.yaml
extends: article
fields:
- header.project
  - .notes

# templates

```sh
templates
├── _articles
│   ├── project-excerpt.html.twig
│   └── project.html.twig
├── _json-ld
│   └── project.html.twig
└── project.html.twig
```

# scaffolds

```sh
scaffolds
└── project.md
```

# scss

```sh
scss
├── articles
│   └── _project.scss
├── templates
│   └── _project.scss
└── project.scss
```

# assets

```sh
assets
├── project.css
├── project.css.map
└── project.js
```

# languages

```sh
languages
└── en.yaml
```


## Installation

- all photon plugins are installed as git submodules. More on that later.



## Configuration


## Usage

Select template type when creating a new page

## Credits


## To Do

- [ ] Future plans, if any


copyright &copy; 2020
