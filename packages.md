
important packages:
    sudo apt install -y zsh git curl fzf

use zsh!
    curl -sS https://starship.rs/install.sh | sh -s -- -y

autosuggestions ofc:
    git clone https://github.com/zsh-users/zsh-syntax-highlighting ~/.zsh/zsh-syntax-highlighting
    git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions

file ~/.zshrc setting:

    eval "$(starship init zsh)"

    source ~/.zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
    source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
    ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=8'

    ZSH_HIGHLIGHT_STYLES[command]='fg=green'
    ZSH_HIGHLIGHT_STYLES[unknown-token]='fg=red,bold'
    ZSH_HIGHLIGHT_STYLES[commandseparator]='fg=blue'   # | и ;
    ZSH_HIGHLIGHT_STYLES[single-hyphen-option]='fg=cyan'
    ZSH_HIGHLIGHT_STYLES[double-hyphen-option]='fg=cyan'
