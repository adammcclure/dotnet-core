# .NET Core SDK 1.0 rc4 build 004771

The installers and binary archives on this page include .NET Core 1.0 SDK RC 4. [Checksums](https://builds.dotnet.microsoft.com/dotnet/checksums/1.0.3-SDK-RC4-4771-SHA.txt) are available to verify downloads.

| .NET Core 1.0 RC 4                        | SDK Installer                                        | SDK Binaries                                        | Runtime Installer | Runtime Binaries | Docker Images |
| ----------------------- | :----------------------------------------------: | :----------------------------------------------:| :--: | :--: | :--: |
| Windows                 | [32-bit](https://go.microsoft.com/fwlink/?linkid=841695) / [64-bit](https://go.microsoft.com/fwlink/?linkid=841686) | [32-bit](https://go.microsoft.com/fwlink/?linkid=841690) / [64-bit](https://go.microsoft.com/fwlink/?linkid=841683) | [32-bit](https://go.microsoft.com/fwlink/?LinkID=836288) / [64-bit](https://go.microsoft.com/fwlink/?LinkID=836279) | [32-bit](https://go.microsoft.com/fwlink/?LinkID=836294) / [64-bit](https://go.microsoft.com/fwlink/?LinkID=836286) | [1.1.0-sdk-msbuild-rc4-nanoserver](https://hub.docker.com/r/microsoft/dotnet/)|
| macOS                   | [64-bit](https://go.microsoft.com/fwlink/?linkid=841693) | [64-bit](https://go.microsoft.com/fwlink/?linkid=841692)                          | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836292) | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836277) | - |
| CentOS 7.1              | -                                                         | [64-bit](https://go.microsoft.com/fwlink/?linkid=841688)                          | - | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836285) | - |
| Debian 8                | -                                                         | [64-bit](https://go.microsoft.com/fwlink/?linkid=841689)                          | - | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836295) | [1.1.0-sdk-msbuild-rc4](https://hub.docker.com/r/microsoft/dotnet/)|
| Ubuntu 14.04            | See notes below for Ubuntu 14.04 and Mint 17 installers   | [64-bit](https://go.microsoft.com/fwlink/?linkid=841687)                         | - | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836278) | - |
| Ubuntu 16.04            | See notes below for Ubuntu 16.04 and Mint 18 installers   | [64-bit](https://go.microsoft.com/fwlink/?linkid=841684)  | - | [64-bit](https://go.microsoft.com/fwlink/?LinkID=836290) | - |

## Installation from a binary archive

When using binary archives to install, we recommend the contents be extracted to /opt/dotnet and a symbolic link created for dotnet. If an earlier release of .NET Core is already installed, the directory and symbolic link may already exist. Ubuntu and Mint users should follow the instructions in the Ubuntu Installation section below.

```bash
sudo mkdir -p /opt/dotnet
sudo tar zxf [tar.gz filename] -C /opt/dotnet
sudo ln -s /opt/dotnet/dotnet /usr/local/bin
```

## Ubuntu installation

dotnet-host-ubuntu-x64.deb
dotnet-hostfxr-ubuntu-x64.deb
dotnet-sharedframework-ubuntu-x64.deb
dotnet-sdk-ubuntu-x64.1.0.0-rc4-004771.deb

### Set up package source

The first step is to establish the source feed for the package manager. This is only needed if you have not previously set up the source or if you are installing for the first time.

#### Ubuntu 14.04 and Linux Mint 17

```bash
sudo sh -c 'echo "deb [arch=amd64] https://apt-mo.trafficmanager.net/repos/dotnet-release/ trusty main" > /etc/apt/sources.list.d/dotnetdev.list'
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 417A0893
sudo apt-get update
sudo apt-get install dotnet-dev-1.0.0-rc4-004771

```

Installed packages

```bash
dotnet-host-ubuntu-x64.1.0.1.deb
dotnet-hostfxr-ubuntu-x64.1.0.1.deb
dotnet-sharedframework-ubuntu-x64.1.0.3.deb
dotnet-sdk-ubuntu-x64.1.0.0-rc4-004771.deb
```

#### Ubuntu 16.04 and Linux Mint 18

```bash
sudo sh -c 'echo "deb [arch=amd64] https://apt-mo.trafficmanager.net/repos/dotnet-release/ xenial main" > /etc/apt/sources.list.d/dotnetdev.list'
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 417A0893
sudo apt-get update
sudo apt-get install dotnet-dev-1.0.0-rc4-004771
```

Installed packages

```bash
dotnet-host-ubuntu.16.04-x64.1.0.1.deb
dotnet-hostfxr-ubuntu.16.04-x64.1.0.1.deb
dotnet-sharedframework-ubuntu.16.04-x64.1.0.3.deb
dotnet-sdk-ubuntu.16.04-x64.1.0.0-rc4-004771.deb
```
