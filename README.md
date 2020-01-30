# setup-win
Set up a fresh Windows 10 install the easy way using Chocolatey (the package manager... It's like a nerdier Ninite?)

Fork and change it to your favourite apps. Mine will be a fairly minimal gaming rig.

## Install [Chocolatey](https://chocolatey.org/install)

1. Open **Windows Powershell** as Administrator
2. Install Chocolatey with the command: `Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`
3. Close and reopen Powershell, or open CMD as Admin, instead.
4. Check it worked with `choco`

**Keep things updated:**

- Keep everything up to date with `choco upgrade all`
- Lock certain apps to a version with `choco upgrade all --except="'speccy,vlc'"` 

## Install Dashlane and Authy

```bash
choco install -y dashlane authy-desktop
```

## Install Firefox and other Utils

```bash
choco install -y vlc 7zip ccleaner firefox speccy
````

## Install Game launchers and Chat clients

```bash
choco install -y discord origin steam uplay goggalaxy vortex epicgameslauncher
```

## Web apps

- [Steam Grid DB](https://www.steamgriddb.com) - add custom banners and logos for your non-steam games.
