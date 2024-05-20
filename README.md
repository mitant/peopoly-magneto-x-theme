# peopoly-magneto-x-theme
A MainsailOS theme for Peopoly Magneto X 3D Printers

# Installation

1. SSH into your Magneto X's pi
2. Clone this repo into a new .theme folder inside your printer's config directory.
```
git clone https://github.com/mitant/peopoly-magneto-x-theme ~/printer_data/config/.theme
```

3. Update your moonraker.conf at ~/printer_data/config/moonraker.conf with the following entry and then you can use the moonraker update interface to update.

```
[update_manager PeopolyMoonrakerTheme]
type: git_repo
primary_branch: main
path: ~/printer_data/config/.theme
origin: https://github.com/mitant/peopoly-magneto-x-theme.git
is_system_service: False
```