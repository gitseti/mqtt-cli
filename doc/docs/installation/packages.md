---
layout: default
title: Packages
parent: Installation
nav_order: 1
---

{:.main-header-color-yellow}
# Installation using a package manager
*** 

## Homebrew
For **Mac OS X** and **Linux** systems use **[Homebrew](https://brew.sh/)** to install MQTT CLI via the **[MQTT CLI Tap](https://github.com/hivemq/homebrew-mqtt-cli)**.
```
$ brew install hivemq/mqtt-cli/mqtt-cli
```


> **NOTE**: If you encounter an error like `Java 1.8+ is required to install this formula` please install a java version higher than 1.8. 
You can use `brew cask install adoptopenjdk` to install the latest release of adoptopenjdk.    

> **NOTE**: As latency-issues may slow down the CLI under **Mac OS X** please verify that you have the entry ``127.0.0.1 localhost your-pc-name`` specified under ``/etc/hosts``.
You can use ``sudo sh -c "echo 127.0.0.1 localhost $(hostname) >> /etc/hosts"`` to append this configuration to your hosts file.

***

## Windows Zip

Download the [Windows Zipfile](https://github.com/hivemq/mqtt-cli/releases/download/v4.6.1/mqtt-cli-4.6.1-win.zip) and extract it in your preferred location.
To execute MQTT CLI simply open the Windows Command Prompt with `⊞ Win` + `R` and execute `cmd`.
Navigate into the extracted MQTT CLI folder and execute `mqtt-cli.exe`.

To quick start the shell simply double-click the `mqtt-cli-shell.cmd` file.

***

## Debian Package

If you are using a *nix operating system which operates with debian packages you can download the MQTT CLI debian package from the [releases page](https://github.com/hivemq/mqtt-cli/releases) via `wget` or `curl` 
and install the package with `sudo dpkg -i`  or `sudo apt install`:


``` 
wget https://github.com/hivemq/mqtt-cli/releases/download/v4.6.1/mqtt-cli-4.6.1.deb
sudo apt install ./mqtt-cli-4.6.1.deb
``` 

***

## RPM Package

For Red Hat, Fedora, Mandriva, OpenSuse, CentOS distributions you can use the rpm package provided at [releases page](https://github.com/hivemq/mqtt-cli/releases).
The preferred way is to install the package via the `yum` package manager. To install the package simply execute:

``` 
sudo yum install -y https://github.com/hivemq/mqtt-cli/releases/download/v4.6.1/mqtt-cli-4.6.1.rpm
```

