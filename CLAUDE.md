# tmux config repo

Personal tmux configuration files.

## Layout
- `tmux.conf` - main config, keybindings, plugin list (TPM format)
- `custom.conf` - sourced at end of `tmux.conf` for machine-local overrides
- `.gitmux.conf` - config for gitmux status segment
- `plugins/` - TPM-managed plugins, cloned locally, not tracked in git except `tpm` itself

## Plugin manager
Plugins declared with `set -g @plugin '...'` in `tmux.conf`, installed via TPM
(`plugins/tpm`). Install/update with prefix + `I` inside a running tmux session.

## Conventions
- Keep plugin declarations grouped together, comment on the same line explaining
  what a non-obvious plugin does
- `run '~/.config/tmux/plugins/tpm/tpm'` must stay the last line in `tmux.conf`
