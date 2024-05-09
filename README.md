# PKGBUILDS

`PKGBUILDS` is a collection of PKGBUILD made specifically for my ArchLinux setup, should work on any ArchLinux-based operating system.

## Usage

### Manual

1. Clone this repository: `git clone https://github.com/null2264/pkgbuilds.git`
2. Navigate to the directory of the PKGBUILD script you want to use: `cd pkgbuilds/<package>`
3. Build and install the package: `makepkg -si`

### Paru

1. Add this repository to Paru config (should be located at `$XDG_CONFIG_HOME/paru/paru.conf`):

   ```conf
   [z]
   Url = https://github.com/null2264/pkgbuilds/
   ```

2. Sync the repo with `paru -Sy --pkgbuilds`
3. Install a package you want to install: `paru -S <package>` or `paru -S z/<package>` to specify the repo
