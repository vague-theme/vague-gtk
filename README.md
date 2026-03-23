<div align="center">
  <img height="80" alt="icon" src="https://github.com/vague-theme/vague/blob/main/assets/icon.png?raw=true" />
  <h1>Vague for GTK</h1>
  <img width="1920" height="1080" alt="Preview" src="https://github.com/user-attachments/assets/10bc1298-15d9-47e5-bd35-f2d3d9aa8796" />
</div>

## Usage

Git clone the repo and paste the theme's folder into your `~/.themes` directory:

```bash
git clone https://github.com/vague-theme/vague-gtk.git
cd vague-gtk
cp -r Vague ~/.themes
```

If `~/.themes` is missing, you can make one:

```bash
cd
mkdir .themes
```

### Switching to theme

You can use the following tools to switch to the theme:
  - Wayland: `nwg-look`
  - Xorg: `lxappearance`

#### GTK 4.0 fix

After switching, symlink to dark to make sure you get the dark mode:

```bash
ln -sf ~/.themes/Vague/gtk-4.0/gtk-dark.css ~/.config/gtk-4.0/gtk.css
```
