# Install oh-my-zsh

https://ohmyz.sh

# Install Powerlevel10K theme

https://github.com/romkatv/powerlevel10k#oh-my-zsh

> Install "Menlo" font and do the initial configuration using `p10k configure` (it is usually auto-launched)

All steps are clearly indicated in the github repo link above.

# Install additional plugins

Below two plugins are present in `.zshrc` plugins list, but not part of `.oh-my-zsh/plugins` directory.
Fix the issue by using below commands

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

# For Git Status Tracking

https://github.com/romkatv/gitstatus#using-from-zsh

```bash
git clone --depth=1 https://github.com/romkatv/gitstatus.git ~/gitstatus
echo 'source ~/gitstatus/gitstatus.prompt.zsh' >> ~/.zshrc
```

Content from above link is already part of `.zshrc` file in the repo.
But do the `git clone` if trying on a different laptop.
No need for `source` command, as the command is part of `.zshrc` already.
