# cli-files

Instructions to setup command line configurations.

## `zsh` configurations

List the commands used to setup `zsh`

### Install Oh-My-zsh to manage configs

	# Install oh-my-zsh
	curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh; zsh

The local copy of "oh-my-zsh" is just as snapshot of the version I currently use.

### Install custom plugins
	
	# Install zsh-syntax-highlighting
	git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
	
	# Install zsh-autosuggestions
	git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
	
	# Install fuzzy finder (answer "y" to all questions)
	git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install
	
	# Install Powerlevel10k (a theme that supports icons and save repetitive commands like `git status`)
	git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k