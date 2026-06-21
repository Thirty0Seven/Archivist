# Archivist

**Version:** v1.2.0 &nbsp;|&nbsp; **Platform:** Linux &nbsp;|&nbsp; **License:** MIT

A simple tool that packages directories into self-extracting shell scripts. That's all there really is to it.

When run, it uses `zenity` for graphical folder selection and outputs a ready-to-go `.sh` file in the same directory as the source. I built this to simplify the process of making these kinds of archives — feel free to tinker with it!


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

Download the `.desktop` file from the project's Releases page and place it wherever you keep your application launchers. When you run it, it pulls `Archivist-Installer.run` straight from the project's GitHub repository and runs it for you — no manual downloading or `chmod`-ing required.

---

## 🔄 Seamless Updates

No need to constantly check for updates yourself. The `.desktop` shortcut stays static on your end, but it always pulls the latest `Archivist-Installer.run` from GitHub before running it — and that script automatically searches for the most recent version tag to install. You will never need to redownload the `.desktop` file again.

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
