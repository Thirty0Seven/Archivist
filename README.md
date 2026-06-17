# Archivist

**Version:** Latest Release &nbsp;|&nbsp; **Platform:** Linux &nbsp;|&nbsp; **License:** MIT

A simple tool that packages directories into self-extracting shell scripts. That's all there really is to it.

When run, it uses `zenity` for graphical folder selection and outputs a ready-to-go `.sh` file in the same directory as the source. I built this to simplify the process of making these kinds of archives — feel free to tinker with it!

> ⚠️ **Note:** This is the first release, so please don't expect too much just yet!

---

## ✨ Features

- **Zero Fuss** — Turn any local folder into a portable, executable shell script archive.
- **GUI-Driven** — Uses simple native dialogs via `zenity` for choosing your source directories.
- **Portable Output** — The resulting self-extracting script can be shared easily and extracted anywhere on Linux.

---

## 📋 Prerequisites

To install and run Archivist, your Linux system needs the following tools:

- **`zenity`** — for the graphical interface
- **`unzip`** — required by the installer to unpack the application assets
- **`curl`** — to fetch the online payload

### Installing Prerequisites

On an **Arch-based** system, grab them via `pacman`:

```bash
sudo pacman -S zenity unzip curl
```

On **Debian/Ubuntu/SteamOS (Desktop Mode)**:

```bash
sudo apt update && sudo apt install zenity unzip curl
```

---

## 🚀 Quick Installation

You can deploy Archivist straight to your system using the unified installer script. From the project's Releases page, download `Archivist-Installer.run`, then run the following in your terminal:

```bash
# Make the installer executable
chmod +x Archivist-Installer.run

# Run the installer framework
./Archivist-Installer.run
```

The installer opens a menu that lets you **install** the desktop shortcut and application binaries cleanly into your user space, or **delete/uninstall** them completely later on if needed.

---

## 🔄 Seamless Updates

No need to constantly check for installer updates. The desktop/front-end side of the installer handles everything statically — if the project gets an update down the road, the installer's back-end references update automatically. You will never need to redownload the local installer file again.

---

## 📦 Legacy Builds

Older builds remain available as legacy options, but these must be installed manually. It's not too difficult:

1. Download the specific `Archivist_assets.zip` from your desired release.
2. Extract the contents directly into your default system directories.
3. **Important:** Manually update the absolute execution and icon paths inside the `.desktop` launcher file, since the installer backend normally handles that automation for you.

---

Hope you have fun!

— 37

*P.S., stay in school, kids.*
