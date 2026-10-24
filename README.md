# WSL Jupyter Kernel

## python, c++, javascript, bash

> do first to install Miniforge3

# Check whether WSL is installed

wsl --status

wsl --list --verbose

wsl --list --online

wsl --install -d Ubuntu


# inside Ubuntu on WSL 2

sudo apt update

sudo apt upgrade -y

# Step 2 — Install Miniforge inside Ubuntu

## 2.1 Download Miniforge

cd ~

wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh

## 2.2 Install it

bash Miniforge3-Linux-x86_64.sh -b -p "$HOME/miniforge3"

## 2.3 Activate Conda

eval "$("$HOME/miniforge3/bin/conda" shell.bash hook)"

conda --version
