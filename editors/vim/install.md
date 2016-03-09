---
layout: section
order: 2
title: Installation
---

1. Install Python's `websocket-client` so the plugin can communicate with ENSIME server.
    ```bash
    $ sudo pip install websocket-client
    ```
1. Export `$BROWSER` if you want to launch documentation directly from Vim. Adding this line to your `.bashrc` for example:
    ```bash
    $ export BROWSER=firefox
    ```
1. Globally install the `ensime-sbt` plugin. This will automatically create the `.ensime` config file for a project.
   Look how to do this [here](https://github.com/metadoc/poms).
1.  Add Ensime-Vim to your plugin manager of choice in your `.vimrc` or `init.vim`

Plugins                                           |Your .{n}vimrc
--------------------------------------------------|-------------------------------
[Vim-Plug](https://github.com/junegunn/vim-plug)  | `Plug 'ensime/ensime-vim'`
[Vundle](https://github.com/VundleVim/Vundle.vim) | `Plugin 'ensime/ensime-vim'`
  
  Under the hood this is just another vim plugin, so other plugin managers should work great as well.

1. If you use NeoVim, make sure you've installed the `neovim` python module
   ```
   $ pip install neovim
   ```
1. After this, update your configuration and install them. With `vim-plug` this is done
by executing `:PlugInstall` followed by `:UpdateRemotePlugins`. With `Vundle` run `:PluginInstall`.
