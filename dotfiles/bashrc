# Add personal scripts to path
export PATH=~/bin:$PATH

# Add current directory to path
export PATH=.:$PATH

# Paths setup for ruby / rails
export PATH="/usr/local/bin:/usr/local/sbin:$PATH"

# Load any bin dir off the working dir.
# This was specifically added to use "bundle exec" bin files when in a rails repo.
export PATH=./bin:$PATH

# Define bash colours
source ~/bin/dotfiles/bash_colours.bash

# Setup Git completion
source ~/bin/dotfiles/git-completion.bash

export CLICOLOR=1
export EDITOR="mate -w"

# Configure prompt
export GIT_PS1_SHOWDIRTYSTATE=true
export PS1="\[$IGreen\]\n\h:\w \[$Yellow\](\$(~/.rvm/bin/rvm-prompt v p g s)) \[$Yellow\]\$(__git_ps1 [%s]) \[$BIGreen\]\n→ \[$Color_Off\] "

# Load RVM
[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm"

# Aliases
alias rm='rm -i'
alias g='git'
function rails_template() { rails new "$@" -J -T -m https://raw.github.com/mitch101/Rails-3-Starter-Kit/master/template.rb; }

# Load custom bashrc
source ~/bin/custom_dotfiles/bashrc


