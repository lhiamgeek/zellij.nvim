# zellij.nvim

neovim integration with [zellij](https://github.com/zellij-org/zellij)
capable of create new pane with PWD of neo-tree

## Features

* `:ZellijNavigate<Left|Right|Down|Up>`
* `:ZellijNewPane`
* `:ZellijNewTab`
* `:ZellijRenamePane`
* `:ZellijRenameTab`

For [vim-tmux-navigator](https://github.com/zellij-org/zellij) compatibility, use the `vimTmuxNavigatorKeybinds` prop during setup.

```lua
use {
    'lhiamgeek/zellij.nvim',
    config = function()
        require('zellij').setup({})
    end
}
```

## Options

```lua
{
    -- keys with designated default values.
    path = "zellij", -- Zellij binary path
    replaceVimWindowNavigationKeybinds = false, -- Will set keybinds like <C-w>h to left
    vimTmuxNavigatorKeybinds = false, -- Will set keybinds like <C-h> to left
    debug = false, -- Will log things to /tmp/zellij.nvim
}
```
