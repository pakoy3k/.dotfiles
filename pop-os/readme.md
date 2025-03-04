The following example saves the above Dconf directories to two files keybindings.dconf and custom-keybindings.dconf and then restores them from the same files:

## Export
> dconf dump '/org/gnome/desktop/wm/keybindings/' > keybindings.dconf

>dconf dump '/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/' > custom-keybindings.dconf

## Restore

> dconf load '/org/gnome/desktop/wm/keybindings/' < keybindings.dconf

> dconf load '/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/' < custom-keybindings.dconf