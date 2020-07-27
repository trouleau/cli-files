# cli-files

Instructions to setup command line configurations.

## `zsh` configurations

List the commands used to setup `zsh`

### Install Oh-My-zsh to manage configs

	# Install oh-my-zsh
	curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh; zsh

The local copy of "oh-my-zsh" is just as snapshot of the version I currently use.

### Install font with icon support

- Go to `https://www.nerdfonts.com/`.
- Download "Meslo Nerd Fond".
- Set "MesloLGSDZ Nerd Font Mono" as profile font in iTerm2.

### Install custom plugins
	
	# Install zsh-syntax-highlighting
	git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
	
	# Install zsh-autosuggestions
	git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
	
	# Install fuzzy finder (answer "y" to all questions)
	git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install
	
	# Install Powerlevel9k (a theme that supports icons and save repetitive commands like `git status`)
	git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k

