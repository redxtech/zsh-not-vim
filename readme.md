# not-vim
> not-vim is a zsh plugin that provides a function that shames the user for forgetting they weren't in vim

## Installing

### zinit
Add this to your zinit config (.zshrc):
```zsh
zinit light redxtech/zsh-not-vim

# it also works with turbo mode:
zinit ice wait lucid
zinit load redxtech/zsh-not-vim
```

### oh-my-zsh
Install it with your favourite zsh package manager, or clone it directly to your
`$ZSH_CUSTOM/plugins` directory with git, and add `zsh-not-vim` to the plugins
array in your `.zshrc` file:

```zsh
plugins=(... zsh-not-vim)
```

## Usage
`not-vim` is very easy to use, simply run the command:

```zsh
not-vim
```

This is mainly used by aliasing `:q`, `:w`, and `:x` to `not-vim`, (automatcally
handled by this plugin) so if you accidentally try to run one of those commands
in the shell, you will be made aware!

I made this because when I was getting started with neovim I found myself
trying to run `:q` or `:x` to close my shell, and I wanted a humourous way
of reminding myself that I was not in vim. I converted it into a plugin
in case anyone else had the same experience.

## Config
You are able to change the program that `zsh-not-vim` used to shame you for
forgetting that you aren't in vim (by default it uses `cowsay`).
For example, to use `yosay` instead, add this line to your `.zshrc`:

```zsh
zstyle :plugins:not-vim say yosay
# to use different cowsay options:
zstyle :plugins:not-vim say cowsay -f vader
```

`zsh-not-vim` will pipe the text into whatever command you specify with this
options and will print the result to `stdout`.

## Demo
[![asciicast](https://asciinema.org/a/aFvn7VWVfuNcbccq2b6pfIce5.svg)](https://asciinema.org/a/aFvn7VWVfuNcbccq2b6pfIce5)

## Author
**not-vim** © [Gabe Dunn](https://github.com/redxtech), Released under the [MIT](./license.md) License.

