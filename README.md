# setup-win

Here is a small guide to get your Windows setup with a list of commmonly used software catered towards a motion designer/content creator using Chocolatey package manager. Alternatively, you can use [Ninite](https://ninite.com/) which has a simpler user interface to install software of your choice.

## [Windows Activation](https://github.com/massgravel/Microsoft-Activation-Scripts/releases/tag/1.8)
### [Bypass Windows 11 Internet Connection & Microsoft Account Login During Setup](https://youtu.be/LX8vb48oodI)
1. Press `Shift + F10` to bring up the Administrator command prompt.
2. Type the following command and press enter: `oobe\BypassNRO`
3. Windows will reboot and you can go through the OOBE section and on the internet connection screen you can choose "I don't have an internet connection" and proceed to create an offline account.
4. When finished you can install the WiFi or Ethernet adapter drivers from a USB stick or CDrom

### License Activation
1. Open **Windows Powershell** as Administrator
2. Copy and paste the code below, and hit enter.
```
irm https://massgrave.dev/get | iex 
```
3. You will see the activation options, and follow onscreen instructions.

## 🍫 Install [Chocolatey](https://chocolatey.org/install) Package Manager

1. Open **Windows Powershell** as Administrator
2. Install Chocolatey with the command: 
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```
3. Close and reopen Powershell, or open CMD as Admin, instead.
4. Check it worked with `choco`

**Keep things updated:**

- Keep everything up to date with `choco upgrade all`
- Lock certain apps to a version with `choco upgrade all --except="'speccy,vlc'"` 

**List all installed packages + versions:**

```bash
choco version all
```




# Step-by-step


## 🌍 Install Browser

```bash
choco install -y chrome vivaldi
````

## 🦜 Install chat clients

```bash
choco install -y discord slack zoom 
```

## 🛠 Install utilities
```bash
choco install -y libreoffice powertoys sharex 7zip quicktime vlc spotifysumatrapdf adobereaderdropbox coretemp windirstat cpu-z imagemagick searcheverything speccy googledrive ffmpeg
```
``` winget install "FFmpeg (Essentials Build)"```



## Install other misc. bits


```bash
choco install -y zotero

```
- [Restoring Zotero Preferences](https://www.zotero.org/support/zotero_data)

## 📺 Install Drivers (Choose one)
- [MSI](https://www.msi.com/support/download/)
### Graphics
- [NVIDIA Experience](https://www.nvidia.com/Download/index.aspx)
- [AMD Adrenaline](https://www.amd.com/en/support)


## ⭐️ Creative
```bash
choco install -y epicgameslauncher obs obs-studio figma miro pureref
```
- [Adobe Creative Cloud](https://www.adobe.com/creativecloud/desktop-app.html)
- [Maxon](https://www.maxon.net/en/maxon-one)
- [Da Vinci Resolve (Sign-up required)](https://www.blackmagicdesign.com/products/davinciresolve/#global-footer)

- [Posthaste](https://www.digitalrebellion.com/posthaste/)
- [PureRef](https://www.pureref.com/download.php)


## 🐧 Install Code Development (Optional)
```bash
choco install -y visualstudiocode git
```
- [Python](https://www.python.org/downloads/windows/)
- [Python setup for VSC}(https://stackoverflow.com/questions/58754860/cmd-opens-windows-store-when-i-type-python)

## Extra stuff (Optional)
- Google Drive
- Dropbox

## Web apps
- uTorrent
