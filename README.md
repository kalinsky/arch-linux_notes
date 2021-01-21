# arch-linux_notes
This is only for keeping notes for the Arch linux installation

To start, first the most important part is knowing what to install to your system. The following packages will contain KDE environment, drivers and linux system. **Please also keep in mind that these packages are Nvidia specific.**

Before chrooting:

> **pacstrap /mnt base linux linux-firmware linux-headers [intel/amd]-ucode networkmanager sudo nano plasma dolphin kate konsole firefox nvidia-dkms nvidia-settings base-devel git grub efibootmgr os-prober gnome-keyring ntfs-3g noto-fonts noto-fonts-cjk noto-fonts-emoji noto-fonts-extra libappindicator-gtk3 bluez bluez-utils**

**[intel/amd]-ucode** - Based on your CPU, choose either **amd-ucode** or **intel-ucode**

**nvidia-dkms nvidia-settings** - Only for Nvidia


Gaming MUST install packages:

### Nvidia
> **nvidia-utils lib32-nvidia-utils vulkan-icd-loader lib32-vulkan-icd-loader**

### AMD
> **lib32-mesa vulkan-radeon lib32-vulkan-radeon vulkan-icd-loader lib32-vulkan-icd-loader**

### General
> **lib32-gnutls lib32-libldap lib32-libgpg-error lib32-sqlite lib32-libpulse**
