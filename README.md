<!--
 Copyright (c) 2022 Neşet Aydın
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

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
1. [First tutorial: Create first project and print Hello, Aliens! ](https://github.com/nesetaydinn/csharp_tutorials/blob/main/first_tutorial/first_tutorial_doc.md)

## LICENSE

[MIT License](LICENSE)

Copyright (c) 2022 Neşet Aydın

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.