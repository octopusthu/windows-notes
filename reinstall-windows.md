# Reinstall Windows

## Back up files

- D:\dev
- Dropbox, Seafile
- Steam

## Back up data and configurations

- Git
  - `%USERPROFILE%\.gitconfig`
  - `%USERPROFILE%\.git-credentials`
- Visual Studio Code
  - Managed by `Settings Sync` via GitHub Account
- Maven
  - Settings
  - Local Repository
- WeChat
- Windows Terminal
- winget
- WSL
- Environment Variables
- Microsoft Store
- Windows Settings

## Just before reinstallation

- Update Intel ME
- Upgrade BIOS
- Set up BIOS
  - Load Optimized Defaults
  - Enable Intel VMX
  - Enable Intel TPM

## Reinstall Windows

- Disk Partition
  - C:\ 800G
  - D:\ 600G
  - E:\ 600G

## System Initialization

- Activate Windows
- Windows Update

- Environment Variables

- [Visual Studio Code](https://code.visualstudio.com/download)
  - Sign in with GitHub Account and turn `Settings Sync` on

- Install Microsoft Store Apps
  - `Windows Terminal`

- Install winget packages
  - `winget install --id Git.Git -e --source winget`
  - `7zip.7zip`
  - `Clash for Windows`

- Map NAS Drives Y:\ and Z:\

- Create Users

## Dev

- `mklink D:\.editorconfig %PROJECT_HOME%\config\os-agnostic\HOME\.editorconfig`
- `mklink E:\.editorconfig %PROJECT_HOME%\config\os-agnostic\HOME\.editorconfig`

- Maven
  - `mklink %USERPROFILE%\.m2\settings.xml %PROJECT_HOME%\config\win\HOME\.m2\settings.xml`
- [Github Desktop](https://desktop.github.com/)
- [Jetbrains Toolbox](https://www.jetbrains.com/toolbox-app/)

## Games

## Other Software

- Install Microsoft Store Apps
  - `Adobe Acrobat Reader DC`

- Install winget packages

- [VLC](https://www.videolan.org/vlc/)
- [爱奇艺](https://www.iqiyi.com/)

## Install

- Map Y: and Z:
  - Disable Quota Management
  - Disable indexing?
- WeChat
  - Z:\Documents\WeChat Files\WeChat Files -> E:\WeChat Files
- [Git](https://git-scm.com/download/win)
  - $PATH=$PATH:E:\software\PortableGit\bin
- Steam
- win_reinstall_bak/Telegram -> E:\software\Telegram
- win_reinstall_bak/ other contents
- 企微
- Adobe Acrobat
- draw.io
- Postman
- QQ 音乐
- PotPlayer
- WSL
  - Docker
- Calibre
- Pulse Secure
