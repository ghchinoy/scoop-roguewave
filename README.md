# Scoop Bucket for Rogue Wave Windows Utilities

This repository contains a custom bucket for [scoop.sh](http://scoop.sh/) for installing 
Rogue Wave open source software.

To use this, after installing scoop, open PowerShell and type:

Add the bucket to scoop

```
scoop bucket add roguewave https://github.com/ghchinoy/scoop-roguewave
```

Test that the bucket is present:

```
> scoop bucket list
roguewave
```


The following tools are referenced

* [rwctl](https://github.com/ghchinoy/rwctl) - a CLI for the Rogue Wave API Management platform


Example install of `rwctl`

```
> scoop search rwctl
roguewave bucket:
  rwctl (0.2.1)

> scoop install rwctl
installing rwctl (0.2.1)
loading https://github.com/ghchinoy/rwctl/releases/download/v0.2.1/rwctl-0.2.1-windows.amd64.exe from cache...
warning: no hash in manifest. sha256 is:
9e05c3fd29bb0aa50ef292833aee4ac2f04cea2123d585d3c67459b1c99bd308
linking ~\scoop\apps\rwctl\current => ~\scoop\apps\rwctl\0.2.1
creating shim for rwctl-0.2.1-windows.amd64
rwctl (0.2.1) was installed successfully!

> rwctl-0.2.1-windows.amd64
rwctl is a CLI tool to manage the Rogue Wave API Platform, including
 APIs, Policies, and API platform and portal settings.

Usage:
  rwctl [command]

Available Commands:
  apis        api commands
  apps        app commands
  policies    policies commands
  portal      portal commands
  profile     profile information
  users       users commands
  version     show the current version
  zip         convenience compression

Flags:
  -h, --help   help for rwctl

Use "rwctl [command] --help" for more information about a command.
```

