# Reinstall Windows

## Back up files

- %USERPROFILE%
- %PROJECT_HOME%
- %DEV_HOME%

## Back up app data and configurations

- Windows Terminal
- Git
  - `%USERPROFILE%\.gitconfig`
  - `%USERPROFILE%\.git-credentials`
- Visual Studio Code
  - Managed by `Settings Sync` via GitHub Account
- Maven
  - Settings
  - Local Repository
- WeChat
- QQ
  - `%USERPROFILE%\Documents\Tencent Files`

- Games
  - Sniper Elite 5
    - `%LOCALAPPDATA%\Sniper Elite 5\`
  - Desperados III
    - `%LOCALAPPDATA%\Desperados III\`
  - Hard West 2
    - `%USERPROFILE%\AppData\LocalLow\Ice Code Games\HardWest2`
- Steam

## Back up system data and configurations

- winget
  - `winget export -o %PROJECT_HOME%\windows-notes\misc\20221218-winget-export.json`
  - `%PROJECT_HOME%\windows-notes\misc\20221218-winget-not-exported.txt`
- WSL
- Environment Variables
- Microsoft Store
- Windows Settings
  - Managed by `Accounts > Windows backup`

## Just before reinstallation

- Prepare necessary drivers

- Update Intel ME
- Upgrade BIOS
- Set up BIOS
  - Load Optimized Defaults
  - Enable Intel VMX
  - Enable Intel TPM

## Reinstall Windows

- Disk Partition
  - C:\ 800G
  - D:\ 500G
  - E:\ 600G

## System Initialization

- Activate Windows
- Windows Update

- Install `Windows Terminal` from Microsoft Store

- Install necessary drivers
  - NVIDIA GeForce Game Ready Driver (GRD)
  - `winget install --id Logitech.GHUB -e --source winget`

- Uninstall packages by `winget uninstall`

- `Google Chrome`

- Display Calibration

- Environment Variables
  - set env `%PROJECT_HOME%`

- Input methods

- [Visual Studio Code](https://code.visualstudio.com/download)
  - Sign in with GitHub Account and turn `Settings Sync` on

- `winget install --id Git.Git -e --source winget`
  - `%USERPROFILE%\.gitconfig`
  - `%USERPROFILE%\.git-credentials`

- `winget install --name "Clash for Windows" -e --source winget`
  - `mklink %USERPROFILE%\.config\clash\config.yaml %PROJECT_HOME%\config\os-agnostic\HOME\.config\clash\config.yaml`

- `winget install --id 7zip.7zip -e --source winget`

- Map NAS Drives Y:\ and Z:\
  - Disable Quota Management?
  - Disable indexing?

- Dropbox
- `winget install --id Seafile.Seafile -e --source winget`

- Create Users

## Dev

- `mklink D:\.editorconfig %PROJECT_HOME%\config\os-agnostic\HOME\.editorconfig`
- `mklink E:\.editorconfig %PROJECT_HOME%\config\os-agnostic\HOME\.editorconfig`

- Java
  - `winget install --id Oracle.JDK.17 -e --source winget`
  - `winget install --id AdoptOpenJDK.OpenJDK.11 -e --source winget`
  - set env `%JAVA_HOME%`
  - set env `%PATH%=%JAVA_HOME%;%PATH%`

- Maven
  - `mklink %USERPROFILE%\.m2\settings.xml %PROJECT_HOME%\config\win\HOME\.m2\settings.xml`
  - set env `%PATH%=${MAVEN_HOME}\bin;%PATH%`
  - restore Local Repository

- Spring
  - set env `%SPRING_PROFILES_ACTIVE%=win`

- [Github Desktop](https://desktop.github.com/)
- [Jetbrains Toolbox](https://www.jetbrains.com/toolbox-app/)
- `winget install --name draw.io -e --source winget`
- [Postman](https://www.postman.com/downloads/)

- Node.js
  - `winget install --id OpenJS.NodeJS.LTS -e --source winget`

## Games

- [Steam](https://store.steampowered.com/about/)

## Other Software

- [Adobe Acrobat Reader DC](https://get.adobe.com/reader/)

- Install `WeChat For Windows` from Microsoft Store
  - Configure `WeChat Files` location

- Install `抖音` from Microsoft Store
- QQ
- QQ 音乐
- PotPlayer
- [VLC](https://www.videolan.org/vlc/)
- [爱奇艺](https://www.iqiyi.com/)

- [企业微信](https://work.weixin.qq.com/#indexDownload)

- `winget install --id calibre.calibre -e --source winget`

- win_reinstall_bak/Telegram -> E:\software\Telegram

- WSL
  - Docker
- Calibre
- Pulse Secure
- 百度网盘
