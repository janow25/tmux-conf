#Configuration files for tmux

## Installation

1. Clone the repository:
```bash
git clone https://github.com/janow25/tmux-conf.git ~/.config/tmux
```

2. Source the configuration file:
```bash
tmux source-file ~/.config/tmux/tmux.conf
```

or in tmux with C+b
```bash
:source-file ~/.config/tmux/tmux.conf
```

3. Clone TPM Plugin Manager:
```bash
git clone https://github.com/tmux-plugins/tpm ~/.config/tmux/plugins/tpm
```

4. Clone Catpuccin theme:
```bash
mkdir -p ~/.config/tmux/plugins/catppuccin
git clone -b v2.1.3 https://github.com/catppuccin/tmux.git ~/.config/tmux/plugins/catppuccin/tmux
```

5. Start tmux:
```bash
tmux
```

6. Change Git Editor to nvim
```bash
git config --global core.editor nvim
```

7. Install gitmux (optional)
```bash
wget https://github.com/arl/gitmux/releases/download/v0.11.2/gitmux_v0.11.2_linux_amd64.tar.gz
sudo mkdir /opt/gitmux
sudo tar -C /opt/gitmux -xzf gitmux_v0.11.2_linux_amd64.tar.gz
sudo ln -s /opt /usr/local/bin
```

# Troubleshooting
- If you encounter issues with the configuration, try running:
```bash
tmux kill-server
```
