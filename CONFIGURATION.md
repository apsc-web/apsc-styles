## ⚙️ Configuration Guide

This [Medium article](https://medium.com/@elad/css-architecture-for-multiple-websites-ad696c9d334) details the structure motivation for the SCSS architecture.

- [File Structure](#file-structure)
- [Tips and Tricks](#tips-and-tricks)


## File Structure

```
├── apsc-scss
├── dev
└── dist
```

- ```apsc-sccs``` contains all of the source [Project Folders](#project-folders)
- ```dev``` contains a static boilerplate HTML page for basic element and component styling
- ```dist``` contains minified production CSS files

# Project Folders

Each project folder in apsc-scss will follow the same pattern:

```
├── _config.scss
├── _local.scss
├── project.scss
├── config
│   ├── _breakpoints.scss
│   ├── _cdn.scss
│   ├── _colors.scss
│   ├── _common.scss
│   ├── _containers.scss
│   ├── _directions.scss
│   ├── _layers.scss
│   └── _typography.scss
└── local
    ├── _fonts.scss
    ├── _functions.scss
    ├── _grid.scss
    ├── _icons.scss
    ├── _mixins.scss
    ├── _partials.scss
    ├── _resets.scss
    ├── _utilities.scss
    ├── mixins
    │ 
    ├── partials
    │   ├── 1-elements
    │   ├── 2-components
    |   ├── 3-...
    │   ├── _1-elements.scss
    │   ├── _2-components.scss
    |   └── 3-...
    └── resets
        └── _typography.scss
```

- ```config```: define/override global variables used inthe project
- ``` local```: implement your styles/functions/mixins

## Partials

Components styles are imported from decreasing specifivity (ie. header styles are imported before button styles and before grid layout styles)


## Tips and Tricks

- Use [Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) to format your SCSS code.
- Whenever possible use mixins/functions to make the code more readable and more easily configurable by others.
- Remember to write headers which explain what your function does and the parameters it accepts.
- Follow the [APSC Guide] for tip on writing SCSS.