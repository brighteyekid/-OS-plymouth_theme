

# पवित्र OS - Plymouth Theme

This repository contains the custom Plymouth boot splash theme created for **पवित्र OS**. This theme gives पवित्र OS a distinct boot-up appearance with a custom splash screen, tailored to complement the overall aesthetics of the OS.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
  - [Setting as Default Boot Splash](#setting-as-default-boot-splash)
- [Screenshots](#screenshots)
- [Troubleshooting](#troubleshooting)
- [License](#license)

---

## Overview
The पवित्र OS - Plymouth Theme is designed to provide a unique and visually appealing boot experience for users of पवित्र OS. This theme includes:
- A centered custom background image that loads during system boot.
- A subtle spinning animation in the center of the screen for a refined loading experience.
- A Mac-inspired or Windows-inspired skin, in line with the custom look and feel of पवित्र OS.

This theme can be installed as the default boot splash on any Debian-based Linux distribution, although it has been specially optimized for use with पवित्र OS.

---

## Installation
To install the पवित्र OS Plymouth theme, follow these steps:

1. **Download and Extract**:
   Clone this repository to your local machine and navigate to the Plymouth themes directory:
   ```bash
   git clone https://github.com/brighteyekid/-OS-plymouth_theme.git
   cd -OS-plymouth_theme
   sudo cp -r pavitraos /usr/share/plymouth/themes/
   ```

2. **Set as Default Boot Splash**:
   Use the following commands to set this theme as the default Plymouth theme.

   ```bash
   sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/pavitraos/pavitraos.plymouth 100
   sudo update-alternatives --config default.plymouth
   sudo update-initramfs -u
   ```

3. **Reboot**:
   Restart your system to view the theme in action during the boot sequence.

---

## Setting as Default Boot Splash
1. **Configure Plymouth Theme**:
   After setting up the theme files in the Plymouth themes directory, use:
   
   ```bash
   sudo update-alternatives --config default.plymouth
   ```

   Select **पवित्र OS - Plymouth Theme** from the list of available Plymouth themes.

2. **Update Initramfs**:
   This step ensures that the Plymouth theme is properly loaded on boot. Run:

   ```bash
   sudo update-initramfs -u
   ```

3. **Final Check**:
   To confirm, reboot the system. You should now see the custom पवित्र OS theme during startup.



## Troubleshooting
- **Theme Not Displaying Properly**: Ensure that the image file paths are correctly set in `pavitraos.script` and that the image files exist in the theme directory (`/usr/share/plymouth/themes/pavitraos/`).
- **Black Screen on Boot**: Check that Plymouth is installed and configured correctly. You can re-run `update-initramfs -u` to update the configuration.

---

## License
This theme is licensed under the Apache-2.0 License. See `LICENSE` for more details.

---

