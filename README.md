# zsh-rustup-completion

Oh-my-zsh rustup completion plugin.

Rustup version: 1.11.0 (e751ff9f8 2018-02-13)

## Installation

First clone the repository repo in the custom zsh plugins folder:

``` bash
cd ~/.oh-my-zsh/custom/plugins
git clone https://github.com/pkulev/zsh-rustup-completion.git rustup
```

Open ~/.zshrc, add plugin to plugins and check that autoloading enabled:

``` bash
vim ~/.zshrc
```

Add the plugin to zsh:
``` bash
plugins=(... rustup)
```

Check that autoloading is enabled
``` bash
autoload -U compinit && compinit
```

Reload config:
``` bash
source ~/.zshrc
```

Enjoy it !


## Updating

Completion file depends on rustup version.
For updating completion just execute:

``` bash
./gen-completion.sh
```

Attention! Executing this file may cause repo updating failure.
