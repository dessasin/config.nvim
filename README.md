### Introduction

A starting point for neovim that is:

* Small (~325 lines)
* Single-file
* Documented
* Modular

### Installation
* Backup your previous configuration
* Copy and paste the defaults.nvim `init.lua` into `$HOME/.config/nvim/init.lua`
* start neovim (`nvim`) and run `:PackerInstall`, ignore any error message about missing plugins, `:PackerInstall` will fix that shortly.
* restart neovim

```bash
mv ~/.config/nvim ~/.config/nvimold

```
### Contribution

Pull-requests are welcome. The goal of this repo is not to create a neovim configuration framework, but to offer a starting template which instructs users on the available features. Some things that will not be included:

* Automatic management of language server installation (for that, there is the nix shell)
* Custom language server configuration (efm templates)
* Theming beyond a default colorscheme necessary for LSP highlight groups
* lazy-loading is an anti-pattern (IMO), and frequently breaks plugins. Defaults.nvim should start within 50 ms on modern hardware. Contribute to upstream plugins to optimize startup time instead.

Each PR, especially those which increase the line count, should have a description as to why the PR is necessary.
