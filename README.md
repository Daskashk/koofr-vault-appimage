# Koofr Vault AppImage

This repository contains the configuration to automatically build an AppImage of Koofr Vault using GitHub Actions.

## How it works

This repository uses GitHub Actions to:
1. Clone the official Koofr Vault repository
2. Compile the Rust application
3. Build the web application
4. Package everything into an AppImage

## Downloads

Built AppImages are available in the [Releases](https://github.com/Daskashk/koofr-vault-appimage/releases) section of this repository.

## Manual build

If you prefer to build the AppImage manually:

```bash
# Clone this repository
git clone git@github.com:Daskashk/koofr-vault-appimage.git
cd koofr-vault-appimage

# Install dependencies
pip install appimage-builder

# Build the AppImage
appimage-builder --recipe AppImageBuilder.yml
