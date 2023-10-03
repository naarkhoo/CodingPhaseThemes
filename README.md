# CodingPhaseDark Theme

This theme is compatible with iTerm and versions for other terminals and text editors are planned for the future.

![CodingPhaseDark Preview](https://github.com/codingphasedotcom/codingphase-iterm-theme/blob/master/iterm-screen.png?raw=true)

## Instructions

### 1. Download or Clone Repository

Either download the zip file of the repository and extract it or clone it using git:

```sh
git clone [REPOSITORY_URL]
```

### 2. Install Dependencies using Homebrew

Install rbenv, ruby-build, and ruby using Homebrew:

```sh
brew install rbenv ruby-build
brew install ruby
```

And add rbenv to your path:

```sh
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
```

Add the following configurations to your `~/.zshrc`:

```sh
#CodingPhase
SPACESHIP_PROMPT_ADD_NEWLINE="true"
SPACESHIP_CHAR_SYMBOL="\uf0e7"
SPACESHIP_CHAR_PREFIX="  \uf296  "
SPACESHIP_CHAR_SUFFIX=(" ")
#SPACESHIP_CHAR_COLOR_SUCCESS="yellow"
SPACESHIP_PROMPT_DEFAULT_PREFIX="$USER"
#SPACESHIP_PROMPT_FIRST_PREFIX_SHOW="true"
#SPACESHIP_USER_SHOW="true"
#CodingPhase
```

### 3. Install Spaceship Theme

Clone the repository and symlink spaceship.zsh-theme to your oh-my-zsh custom themes directory:

```sh
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

Add the following aliases from colorls to your `~/.zshrc`:

```sh
alias ls='colorls  --sd'
alias lst="colorls --tree"
alias lsr="colorls --sort-dirs --report"
```
