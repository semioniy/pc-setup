# Install Chocolatey
> https://chocolatey.org/install
## Admin PS:
```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```
# Install packages I need on any system
```powershell
choco install powertoys rambox bitwarden em-client syncthingtray microsoft-windows-terminal googlechrome ublockorigin-chrome bitwarden-chrome 7zip javaruntime obsidian dropbox -y
```
## Only on systems I plan to code on
```powershell
choco install git sourcetree wsl2 docker fluent-terminal nodejs.install intellijidea-community vscode anaconda3 -y
```
# Set up 
## Regular PS:
`notepad $profile` - copy and save:
```powershell
Import-Module $env:ChocolateyInstall\helpers\chocolateyProfile.psm1
```
### Set up python and anaconda
