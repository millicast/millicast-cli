# Millicast CLI Client

This is the command line interface to interact with millicast from your terminal.

## Supported OS

| Windows | MacOs | Linux |
| --- | --- | --- | 
| [x] Win10 | [x] MacOS Catalyna intel | [ ] Ubuntu 18 Deb Package |
|           | [x] MacOS BigSur intel | [x] Ubuntu 20 Deb Package |


## Features

### Autocompletion

| Windows | MacOs | Ubuntu |
| --- | --- | --- |
| [ ] git bash | [ ] bash | [x] bash |
| [ ] CMD | [ ] zsh | [ ] zsh |

### Commands

| list | config | publish | subscribe |
| --- | --- | --- | --- |
| [x] camera sources          | [x] config saved in file  | [x] Blocking mode              | [x] Blocking mode | 
| [x] ndi sources/output      | [x] millicast credentials | [ ] detached mode              | [ ] detached mode | 
| [x] decklink sources/output | [x] media                 | [x] svc                        | [ ] audio control | 
| [x] screen/app sources      | [x] multiconfig           | [x] simulcast                  | [ ] override config parameters | 
| [x] mic sources             | [ ] alias                 | [ ] audio/video control        | [ ] Show / report stats | 
| [x] speakers                |                           | [ ] override config parameters | [x] NDI output | 
| [x] codecs                  |                           | [ ] Show / report stats        | [x] decklink output | 

## Installation

### Windows

First download the msi installer.

Double-Click, follow the instructions.

The installer will install the cli binaries on your machine and modify the path environment variable,
so the binary ``mccli.exe`` will be accessible from your CMD console / git bash.

To check the installation, open a console and run ``mccli help``, this should show you the help.

To uninstall, open your control panel, go into uninstall programs and uninstall millicast-cli.

### Ubuntu

Download the debian package.

Then, open a shell and go in your download directory.

Install the package by running : 

```bash

sudo apt install ./millicast-cli-1.0-Linux.deb

```

This will install the cli and all its dependencies.

Run ``mccli help`` to check if the installation went well.

Note that if you are using bash, you have the autocompletion available.

To uninstall, run : 

```bash

sudo apt remove millicast-cli

```

### Mac

Dowload the tar.gz archive.

Go into your dowload directory and run : 

```zsh

tar zxvf millicast-cli-1.0-Darwin.tar.gz

cd millicast-cli-1.0-Darwin

chmod +x install.sh

./install.sh

```

This will install the cli in ``/usr/local``.

Run ``mccli help`` to check if the installation went well.

To uninstall, run :

```zsh

chmod +x uninstall.sh

./uninstall.sh

```
