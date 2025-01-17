# telescope-rooter

## What is telescope-rooter

`telescope-rooter.nvim` is a extension for the telescope neovim plugin. `telescope-rooter.nvim` changes the working directory to the to the project/root path before the `TelescopePrompt` is started and restores the working directory to the previous once closed.

## Requirements

This plugins requires `telescope.nvim` and `plenary`

## Installation

using packer

```
use("desdic/telescope-rooter.nvim")
```

## Enabling in telescope

```
require "telescope".load_extension("rooter")
```

## Default configuration

```
extensions = {
  ...
    rooter = { 
       enable = true,
       patterns = { ".git" },
       debug = false
    }
}
```

Note that if one of the patterns are not found it will not change the current working directory

## Usage

`telescope-rooter.nvim` can be enabled/disabled using `:Telescope rooter toggle`

## TODO

- automatic testing via github
