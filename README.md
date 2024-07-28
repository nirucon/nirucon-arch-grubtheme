# nirucon-death-grubtheme
## Overview

nirucon-death is a visually striking GRUB2 theme designed to give your bootloader a unique and haunting appearance. The theme features a compelling background image of death, enhancing the visual appeal of your system's startup sequence. Additionally, it includes icon support for several popular Linux distributions, ensuring a cohesive and aesthetically pleasing interface.

## Features

- **Background Image**: An evocative image of death.
- **Distribution Icons**: Custom icons for various Linux distributions, creating a uniform and attractive boot menu.

## Installation Instructions

To install the nirucon-death GRUB2 theme, follow these steps:

1. **Clone the Repository**

   Begin by cloning the repository to your local machine:
   ```bash
   git clone https://github.com/nirucon/nirucon-death-grubtheme
   ```

2. **Copy the Theme Folder**

   Navigate to the cloned repository and copy the theme folder to the GRUB themes directory:
   ```bash
   cd /nirucon-death-grubtheme/nirucon-death
   sudo cp -r nirucon-death /boot/grub/themes/
   ```

3. **Configure GRUB**

   Next, you'll need to edit the GRUB configuration file to use the new theme. Open `/etc/default/grub` with your preferred text editor (e.g., nano):
   ```bash
   sudo nano /etc/default/grub
   ```

   Add or modify the following line to set the theme:
   ```bash
   GRUB_THEME="/boot/grub/themes/nirucon-death/theme.txt"
   ```

4. **Update GRUB**

   Apply the changes by updating GRUB:
   ```bash
   sudo update-grub
   ```

5. **Reboot**

   Finally, reboot your system to see the new theme in action:
   ```bash
   sudo reboot
   ```

## Troubleshooting

- **Missing Icons**: Ensure that the icon files are correctly placed in the theme directory.
- **Configuration Errors**: Double-check the path specified in the `GRUB_THEME` variable.
- **No Theme Applied**: Make sure to run `sudo update-grub` after editing the GRUB configuration file.
