Tetra
======
Tetra (formerly or codenamed "Project Beaucoup") is Adwaita-based gtk+ theme with design influence from elementary OS stylesheet/theme.

-------------------
![Screenshot](/data/Screenshot.png)
![Screenshot](/data/Screenshot-dark.png)
-------------------
This theme has come with **3 variants**

**Variants** | **Description** | **Preview**
:-: | :-: | :-:
**Default** | Light variant with dark panel | ![Default](/data/variant-default.svg)
**Dark** | Dark variant | ![Dark](/data/variant-dark.svg)
**Light** | Light variant with light panel (and GNOME shell theme) | ![Light](/data/variant-light.svg)

# Supported desktop environments
- GNOME 3
- Xfce
- Budgie
- MATE (partial, No WM theme for marco and still not completed.)

### Not supported desktops
- Cinnamon
> ~~Not happening. See you in 2019.~~ Canceled, no plans for Cinnamon support.
- Pantheon
> Elementary OS is NOT compatible.
- LXDE
- Window Managers (Openbox, enlightenment...)
- Qt/Non-gtk+ desktops (Plasma 5, LXQt...)


### Ubuntu 18.10 and later
> ~~Ubuntu 18.10 ships with GNOME 3.30 desktop, but Nautilus file manager is still version 3.26 because that goddamn desktop icons feature, Ubuntu 18.04 (and 16.04*) support will remain, but not for 18.10 since it will broke Nautilus pathbar styling (unless if Ubuntu Desktop/UG team/someone backport Nautilus 3.30 to 18.10 via PPA)
**Update: See ubuntu-1810 branch for special version for Ubuntu 18.10**
**Update2: Deprecated. Ubuntu 18.10 is NOT REALLY, really supported.**~~

**Update (again) :** Nautilus 3.30 is available for Ubuntu 18.10 on [gnome3-team/gnome3-staging ppa](https://launchpad.net/~gnome3-team/+archive/ubuntu/gnome3-staging?field.series_filter=cosmic), so it's **important** to use Nautilus 3.30 to have a better experience on Ubuntu 18.10 **(it will lose desktop icons feature, but you can use desktop icons extension for GNOME shell to restore desktop icon feature)**. Ubuntu 19.04 ships with Nautilus 3.32 w/Desktop icon extension for GNOME shell.

# (GNOME Shell) Typography
**Noto Sans**is used as default primary font for GNOME shell theme, Cantarell is used as fallback.

# Installation
### Dependencies
before you installing this theme, you need this package installed on your system:
- `sassc` for compiling sass css sources
- `gtk` 3.22
- [Ubuntu 16.04 users read this](https://github.com/hrdwrrsk/tetra-gtk-theme/wiki/Ubuntu-16.04-users-read-this)
- `bc` (required before running `install.sh` script)

#### Required for rendering assets
- `inkscape`
- `optipng`

Then run this command:

```
git clone https://github.com/hrdwrrsk/tetra-gtk-theme.git
cd tetra-gtk-theme

# System-wide install
sudo ./install.sh

# Local install
./install.sh -d ~/.themes
```

# Reporting bugs
report it via "Issues" tab, Pull request for bugfixes also accepted.
for suggestion about design add [design] tag, for DEs/gtk+ app theming/etc. support, add [feature request] tag

# Credits
- Adwaita gtk+ theme
- elementary OS stylesheet/gtk+ theme as main inspiration (also color palette.)
- install.sh, parse-sass.sh and render-assets.sh script are from nana-4's materia-theme
- some other projects: Adapta, Arc, plane-gtk-theme, etc.
