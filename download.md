# Download Gitux

Choose your platform and download from the [GitHub Releases](https://github.com/gitux-co/downloads/releases).

## Desktop App

<div class="download-grid">

### Windows
**Gitux for Windows**
- [Download .exe](https://github.com/gitux-co/downloads/releases/latest/download/Gitux-Setup.exe)

### macOS
**Gitux for macOS** (Apple Silicon)
- [Download .dmg](https://github.com/gitux-co/downloads/releases/latest/download/Gitux.dmg)
- [Download .zip](https://github.com/gitux-co/downloads/releases/latest/download/Gitux.zip)

### Linux
**Gitux for Linux**
- [Download .deb](https://github.com/gitux-co/downloads/releases/latest/download/Gitux.deb) (Debian/Ubuntu)
- [Download .flatpak](https://github.com/gitux-co/downloads/releases/latest/download/Gitux.flatpak)

</div>

## System Requirements

| Platform | Minimum Requirements |
|----------|---------------------|
| Windows | Windows 10+, 4GB RAM |
| macOS | macOS 11+ (Apple Silicon), 4GB RAM |
| Linux | Ubuntu 20.04+ or equivalent, 4GB RAM |

## Installation

### Linux

**Debian/Ubuntu:**
Via terminal run the below, or double click the .deb file and click install:
```bash
sudo dpkg -i <path-to-downloaded-file>/Gitux.deb
```

**Flatpak:**
```bash
flatpak install <path-to-downloaded-file>/Gitux.flatpak
```

### Windows
Run the `.exe` installer and follow the prompts.

### macOS
Open the `.dmg` and drag Gitux to your Applications folder.

MacOS will claim the package is broken but it is not, it is just Apple trying to force developers to pay each year for a developer license which is not required for this application.

If macOS blocks the app from opening, run this in Terminal first:
```bash
xattr -cr /Applications/Gitux.app
```

## Licensing

You'll be asked for a license key when you first launch the app.

::: tip Don't have a license yet?
[Purchase Gitux](/pricing) to get your license key instantly via email.
:::

## Updating

Gitux checks for updates automatically. When one's available, you'll see a notification. Click to download, then restart to apply.

## Need help?
Email **support@gitux.co**.
