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

## Config
You are able to change the program that `zsh-not-vim` used to shame you for
forgetting that you aren't in vim (by default it uses `cowsay`).
For example, to use `yosay` instead, add this line to your `.zshrc`:

```zsh
zstyle :plugins:not-vim say yosay
```

`zsh-not-vim` will pipe the text into whatever command you specify with this
options and will print the result to `stdout`.

## Author
**not-vim** © [Gabe Dunn](https://github.com/redxtech), Released under the [MIT](./license.md) License.

