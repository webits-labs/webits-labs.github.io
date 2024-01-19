Now that you have WSL 2.0 installed on your Windows 10 or 11 desktop, here are a few tips and tricks you can use to further enhance your experience


## Basic installation:
wsl --install

## Installation without a default distro
wsl --install --no-distribution

## Install specific distro
wsl --install --debian
wsl --install --kali

## Install WSL 1.0
wsl --install --enable-wsl1

## Install without rebooting:
wsl --install --norestart

## List WSL distributions and which version is running
wsl --list --verbose

## Set default version for a specific distro
wsl --set-version "distroname" "Version"  EX: wsl --set-version debian 2

## Open specific distro
wsl -d "distroname" EX: wsl -d debian

