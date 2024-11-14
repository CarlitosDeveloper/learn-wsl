# Learn WSL with Carlitos

![Header](./src/Wsl_01.webp)

Welcome to this repository, created to help you understand and effectively use Windows Subsystem for Linux (WSL). Here you’ll find notes, guides, and practical tips to set up and manage WSL, with the goal of establishing a solid foundation for using Linux tools directly within a Windows environment.

## General Objectives

- Enable a seamless development environment by using Linux commands and tools within Windows through WSL.

## Specific Objectives

1. **WSL Installation and Setup**
   - Install WSL on Windows 10/11.
   - Set up a preferred Linux distribution in WSL.

2. **Basic Usage and System Management**
   - Learn essential Linux commands to navigate and manage the WSL environment.
   - Understand file sharing and permissions between Windows and WSL.

3. **Development and Package Management**
   - Install and manage development tools and packages within WSL.
   - Set up an integrated workflow between Windows and WSL for development.

## Resources and References

- Visit my YouTube channel for video tutorials on WSL and development: [Developing With Carlitos](https://www.youtube.com/@DevelopingWithCarlitos).
- [WSL Documentation](https://docs.microsoft.com/en-us/windows/wsl/) – Official documentation for WSL.
- [Linux Command Cheat Sheet](https://www.commandlinefu.com) – Commonly used Linux commands and examples.

---

## Commands and Configuration for WSL

### 01 - WSL Installation and Version Commands

| Command                                           | Description                                                             |
| :-----------------------------------------------: | :---------------------------------------------------------------------- |
| `wsl --install`                                   | Installs WSL and the default Linux distribution                         |
| `wsl --install -d <DistroName>`                   | Installs a specific Linux distribution (e.g., Ubuntu)                   |
| `wsl --version`                                   | Displays the version of WSL installed                                   |
| `wsl --update`                                    | Updates WSL to the latest version                                       |
| `wsl --status`                                    | Displays the current status of WSL                                      |
| `wsl --help`                                      | Displays WSL help                                                       |

### 02 - Distribution Management Commands

| Command                                           | Description                                                             |
| :-----------------------------------------------: | :---------------------------------------------------------------------- |
| `wsl --list --online`                             | Lists available Linux distributions for installation                    |
| `wsl --list --verbose`                            | Lists installed distributions with details                              |
| `wsl --set-default <DistributionName>`            | Sets a distribution as the default                                      |
| `wsl --unregister <DistributionName>`             | Uninstalls a specific distribution                                      |

### 03 - Additional Configuration Commands

| Command                                           | Description                                                             |
| :-----------------------------------------------: | :---------------------------------------------------------------------- |
| `wsl --inbox`                                     | Runs WSL from the inbox (advanced option)                               |
| `wsl --no-distribution`                           | Runs WSL without a distribution (advanced option)                       |

### 04 - Session and User Management Commands

| Command                                           | Description                                                             |
| :-----------------------------------------------: | :---------------------------------------------------------------------- |
| `wsl --shutdown`                                  | Shuts down all running WSL instances                                    |
| `wsl --terminate <DistributionName>`              | Terminates a specific distribution instance                             |
| `wsl --user <Username>`                           | Sets a default user                                                     |
| `<DistributionName> config --default-user <Username>` | Configures the default user for a specific distribution             |

### 05 - Useful Commands for Working in WSL

| Command                                           | Description                                                             |
| :-----------------------------------------------: | :---------------------------------------------------------------------- |
| `wsl ~`                                           | Starts a session in the home directory                                  |
| `exit`                                            | Exits the WSL session                                                   |
| `explorer.exe .`                                  | Opens the current WSL directory in Windows Explorer                     |
| `wsl <command>`                                   | Runs a specific Linux command from the Windows command line             |
| `code .` (requires VS Code installed)             | Opens the current WSL directory in Visual Studio Code                   |

### 06 - Basic Linux Commands in WSL

| Command                       | Description                                                                |
| :---------------------------: | :------------------------------------------------------------------------- |
| `ls`                          | Lists files and directories in the current WSL directory                   |
| `cd /path/to/directory`       | Changes the current directory                                              |
| `pwd`                         | Prints the current working directory in WSL                                |
| `mkdir new_folder`            | Creates a new directory                                                    |
| `rm filename`                 | Removes a file                                                             |
| `cp source_file destination`  | Copies a file to a specified destination                                   |
| `mv source destination`       | Moves or renames a file or directory                                       |

### 07 - Development and Package Management Commands

| Command                                   | Description                                                          |
| :---------------------------------------: | :------------------------------------------------------------------- |
| `sudo apt update`                         | Updates the package lists (Debian-based distributions)               |
| `sudo apt upgrade`                        | Upgrades all installed packages                                      |
| `sudo apt install <package_name>`         | Installs a package (Debian-based distributions)                      |
| `sudo apt remove <package_name>`          | Removes an installed package                                         |
| `sudo apt autoremove`                     | Removes unused packages and dependencies                             |

---

This guide will help you get started with WSL, making it easy to integrate Linux tools into your Windows workflow. Explore each command, understand its purpose, and begin building a powerful development environment with WSL!
