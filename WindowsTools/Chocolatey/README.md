# Chocolatey

[Chocolatey](https://chocolatey.org) is a software management solution that allows you to manage 100% of your software, anywhere you have Windows, with any endpoint management tool.

## Installation

From https://chocolatey.org/install

```shell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

## Export installed applications

```shell
choco export "c:\temp\packages.config"
```

## Install applications from config file

```shell
choco install "c:\temp\packages.config"
```

## Upgrade all packages

```shell
choco upgrade all
```

## Create Scheduled Task to upgrade all packages

```shell
schtasks /create /tn "Choco Upgrade All Daily" /tr 'choco upgrade all' /sc daily /st 09:00 /rl HIGHEST
```

## List installed packages

```shell
choco list --localonly 
```
