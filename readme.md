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

## Author
**not-vim** © [Gabe Dunn](https://github.com/redxtech), Released under the [MIT](./license.md) License.

