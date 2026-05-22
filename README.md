# Xibo for Linux (Fork)
[![xibo-player](https://snapcraft.io/xibo-player/badge.svg)](https://snapcraft.io/xibo-player)

Xibo for Linux is a Digital Signage Player for [Xibo](https://xibo.org.uk).

> **Note:** This is a personal fork focused on getting Xibo running on 
> modern hardware with GNOME Wayland on Fedora Workstation. 
> You are welcome to use or build on this code freely, but this is not 
> an actively maintained fork — no issues or pull requests are being managed.
> Treat this as experimental work in progress, not a supported release.


For help, guides, or support please visit the official Xibo community:
 [join our community](https://community.xibo.org.uk/c/support/linux-player).


# Installation

Installation and upgrade instructions can be found [here](https://xibo.org.uk/docs/setup/xibo-for-linux-installation).


## Goal
Get Xibo running natively on GNOME Wayland on modern Fedora hardware.
This is a long term project driven by learning as much as fixing.


## Test Environment
- Fedora Workstation (latest)
- GNOME on Wayland


### Building from source
- Clone this repository
- Run `cmake` in the root of the repository

# Debugging
We provide a VSCode dev container that has everything needed to build/debug the application using VSCode. This devcontainer uses a base image which is built from the `Dockerfile` in the root folder.

To debug this application using VSCode.

1. Copy the settings folder from a working player install into the `/build/bin` folder, making sure you have `cmsSettings.xml` and `playerSettings.xml`. 
2. Open `cmsSettings.xml` and adjust the `localLibrary` setting to be `/workspaces/vscode/build/bin/library`.
3. Open the application directory using the remote containers plugin.
4. Go to the aplication debug extesion at left panel and click on the green play button.

Tutorial video: https://user-images.githubusercontent.com/6628028/162645464-5eadcb2b-a53a-450e-805f-9589fba6f8f0.mp4

[Issue 260](https://github.com/xibosignage/xibo-linux/issues/260) will improve steps 1 and 2 so that the options app can be used.
