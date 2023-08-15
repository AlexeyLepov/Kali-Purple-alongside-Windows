Kali-Purple alongside Windows Installation
====================================================================================================================

Make sure to back up your important data before attempting any installation. 

### `✅ Step 1:` Downloading Kali Linux ISO

- Visit the official Kali Linux [website](https://www.kali.org/downloads/)
- Or use the direct [download link](https://cdimage.kali.org/kali-2023.2/kali-linux-2023.2a-installer-purple-amd64.iso)

### `✅ Step 2:` Create a Bootable USB Drive (or DVD)

- To create a bootable USB drive, you can use software like [Rufus](https://github.com/pbatard/rufus/releases) for Windows or [Etcher](https://etcher.balena.io/).
- Download and install the desired software.
- Connect a USB flash drive (at least `8GB` in size) to your computer.
- Run Rufus or Etcher, select the Kali Linux ISO you downloaded, and choose the connected USB drive as the target.
- Start the process, and it will create a bootable USB drive with Kali Linux.

### `✅ Step 3:`  Allocate free space on your disk

If you intend to use both Windows and Kali Linux systems, you should shrink your Windows virtual disk. A minimum of `20GB` is required:

<div align="center"> 
<img width=100% src="https://github.com/AlexeyLepov/KaliPurpleAlongsideWindows/assets/77492646/b1668e0c-b5e9-4b2b-a699-7d763786d452">
</div>

### `✅ Step 4:` Boot from the Kali Linux USB Drive

- Insert the bootable USB drive into your computer's USB port.
- Restart your computer and enter the BIOS or UEFI settings. The process for accessing BIOS/UEFI varies depending on your computer manufacturer. Usually, you can do this by pressing a key like `Del`, `F2`, `F12`, or `Esc` during boot.
- In the BIOS/UEFI settings, change the boot order to prioritize the USB drive (or DVD drive if you're using a DVD) over the internal storage, or simply override the boot.
- Save the changes and exit the BIOS/UEFI settings using `F10`.

### `✅ Step 5:` Start the Kali Linux Installation

- When your computer restarts, it should boot from the Kali Linux USB drive.
- You'll be presented with the Kali Linux boot menu. Choose the `Graphical Install` option to start the installation process.

<div align="center"> 
<img width=100% src="https://github.com/AlexeyLepov/Kali-Purple-alongside-Windows/assets/77492646/deaa4838-7b8d-4337-be39-77569aea472e">
</div>

### `✅ Step 6:` Configure Kali Linux Installation

- Select your preferred language, location, and keyboard layout, etc.
- Set up your hostname for the Kali Linux system (you can leave the domain empty).
- Create a user with a strong root password.
- Configure the network (you may need to provide details like Wi-Fi credentials if you're using a wireless connection).

### `✅ Step 7:` Partitioning and Disk Setup

- Select the disk you want to use for installation.
- Select the first option: **`Guided - Use the largest continuous free space`**
- Review and confirm the partition changes.

### `✅ Step 8:` Install the System

- The installer will proceed to install Kali Linux onto the selected disk.
- During the installation, you may be asked to set up the system clock and configure the package manager. Choose the appropriate options based on your location and preferences.
- The installer will prompt you to install the GRUB boot loader. Confirm the installation on the same disk where Kali Linux is being installed.

### `✅ Step 9:` Complete the Installation

- Once the installation is complete, the installer will prompt you to remove the installation media (USB/DVD) and press 'Enter' to reboot the system.
- Remove the USB drive or DVD and hit 'Enter' to restart.
- After the system reboots, you'll be presented with the Kali Linux login screen.

### `❗❗ Note: ❗❗` 

If you encounter any problems while at the stage `Select and Install Software` or `Install the Base System`, you should click on the `Go Back` button and try to install the GRUB loader first. After that, click on `Go Back` again and there should be no problem with installing the software.

### `🎉 Congrats! 🎉` 

- You have successfully installed Kali Linux on your system. Remember to keep your system updated and secure by applying regular updates and using Kali Linux responsibly.

- Enter terminal `Ctrl+Alt+T` and type:

```bash
sudo apt-get update
sudo apt-get upgrade
```

- You may also be interested in the [Kali Linux initial setup](https://github.com/AlexeyLepov/Kali-initial-setup). 
