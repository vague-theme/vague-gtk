<div align="center">
  <img height="80" alt="icon" src="https://github.com/vague-theme/vague/blob/main/assets/icon.png?raw=true" />
  <h1>Vague for GTK</h1>
  <img width="1920" height="1080" alt="Preview" src="https://github.com/user-attachments/assets/10bc1298-15d9-47e5-bd35-f2d3d9aa8796" />
</div>

## Usage

Clone the repo and copy the theme into `~/.themes`:

```bash
git clone https://github.com/vague-theme/vague-gtk.git
mkdir -p ~/.themes
cp -r vague-gtk/Vague ~/.themes
```

## Switching themes

### CLI

```bash
# GTK
THEME_DIR="$HOME/.themes/Vague"
mkdir -p ~/.config/gtk-4.0 ~/.config/gtk-3.0 ~/.config/gtk-2.0
ln -sf "$THEME_DIR/gtk-4.0/gtk.css" ~/.config/gtk-4.0/gtk.css
ln -sf "$THEME_DIR/gtk-3.0/gtk.css" ~/.config/gtk-3.0/gtk.css
ln -sf "$THEME_DIR/gtk-2.0/main.rc"  ~/.config/gtk-2.0/main.rc
ln -sf "$THEME_DIR/gtk-2.0/apps.rc"  ~/.config/gtk-2.0/apps.rc
ln -sf "$THEME_DIR/gtk-2.0/hacks.rc" ~/.config/gtk-2.0/hacks.rc

# Desktop Environments
gsettings set org.gnome.desktop.interface gtk-theme "Vague"
gsettings set org.cinnamon.theme name "Vague"
xfconf-query -c xfwm4 -p /general/theme -s "Vague" # XFCE window decorations
```

### GUI

The following tools handle everything, no CLI needed:

- Wayland: `nwg-look`
- Xorg: `lxappearance`
