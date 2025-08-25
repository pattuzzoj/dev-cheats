# Package Managers in Linux

## APT

Package manager used in Debian, Ubuntu, and derivatives.

| Command                | Description                                                        |
| ---------------------- | ------------------------------------------------------------------ |
| apt update             | Updates the list of available packages                             |
| apt upgrade            | Upgrades installed packages to the latest version                  |
| apt full-upgrade       | Upgrades packages and installs/removes dependencies if needed      |
| apt install \[package] | Installs a package                                                 |
| apt remove \[package]  | Removes a package                                                  |
| apt purge \[package]   | Removes a package and its configuration files                      |
| apt autoremove         | Removes automatically installed packages that are no longer needed |
| apt search \[package]  | Searches for available packages                                    |
| apt show \[package]    | Shows details about a package                                      |
| dpkg -i \[file.deb]    | Installs a `.deb` package manually                                 |
| dpkg -r \[package]     | Removes a package installed with dpkg                              |

---

## Pacman

Package manager used in Arch Linux, Manjaro, and derivatives.

| Command               | Description                               |
| --------------------- | ----------------------------------------- |
| pacman -Syu           | Updates the system and all packages       |
| pacman -S \[package]  | Installs a package                        |
| pacman -R \[package]  | Removes a package                         |
| pacman -Rs \[package] | Removes a package and unused dependencies |
| pacman -Scc           | Cleans the package cache                  |
| pacman -Ss \[package] | Searches for available packages           |
| pacman -Qi \[package] | Shows information about a package         |
| pacman -Ql \[package] | Lists files installed by a package        |

---

## DNF / YUM

Package manager used in Fedora, RHEL, and CentOS.

| Command                | Description                                          |
| ---------------------- | ---------------------------------------------------- |
| dnf update             | Updates all packages                                 |
| dnf install \[package] | Installs a package                                   |
| dnf remove \[package]  | Removes a package                                    |
| dnf check-update       | Checks for available updates                         |
| dnf upgrade            | Upgrades installed packages                          |
| dnf clean all          | Cleans the package cache                             |
| dnf info \[package]    | Shows details about a package                        |
| yum install \[package] | Legacy command for installing packages (CentOS/RHEL) |

---

## Zypper

Package manager used in openSUSE and SUSE Linux Enterprise.

| Command                   | Description                     |
| ------------------------- | ------------------------------- |
| zypper refresh            | Updates the package repository  |
| zypper update             | Updates all installed packages  |
| zypper install \[package] | Installs a package              |
| zypper remove \[package]  | Removes a package               |
| zypper search \[package]  | Searches for available packages |
| zypper info \[package]    | Shows details about a package   |
| zypper clean              | Cleans the package cache        |
| zypper patch              | Applies security updates        |

---

## Flatpak

Distribution-independent package system for sandboxed applications.

| Command                            | Description                          |
| ---------------------------------- | ------------------------------------ |
| flatpak install \[repo] \[package] | Installs a package from a repository |
| flatpak update \[package]          | Updates installed packages           |
| flatpak uninstall \[package]       | Removes a package                    |
| flatpak list                       | Lists all installed packages         |

---

## Snap

Canonical’s package system for sandboxed applications.

| Command                 | Description                       |
| ----------------------- | --------------------------------- |
| snap install \[package] | Installs a package                |
| snap remove \[package]  | Removes a package                 |
| snap refresh            | Updates all snap packages         |
| snap list               | Lists all installed snap packages |

---

> ⚠️ Some commands may require administrative privileges.