# csharp_tutorials

## Install dotnet core on Ubuntu 20.04
- 1st Step:
Add package repo
```bash
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
rm packages-microsoft-prod.deb
```
- 2nd Step:
Install dotnet-sdk package
```bash
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-6.0
```
- 3rd Step:
Install aspnet-core runtime package
```bash
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y aspnetcore-runtime-6.0
```
## Install vscode on Ubuntu 20.04 and install some extensions
```bash
sudo snap install --classic code
```
After vscode has been install, touch <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>X</kbd> and install this extensions;
1. C#
2. vscode-icons

## Tutorial docs
1. Fİrst tutorial: Create first project and print Hello, Aliens! <link-come-here>
