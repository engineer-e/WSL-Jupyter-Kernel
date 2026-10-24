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

## 2.4 Create Virtual Environment & Install Jupyter Lab

conda create -n kernels -c conda-forge jupyterlab -y

## 2.5 Activate the Virtual Environment

conda activate kernels

jupyter kernelspec list

## 2.6 Install bash_kernel

python -m pip install --upgrade pip

python -m pip install bash_kernel

## 2.7 Open Jupyter Lab

jupyter lab

![alt text](kernel/image.png)

# Super!!! - Successfully Completed (^o^)


# C++ - Xeus-Cling

> for c++, close the Jupyter lab , Ctrl+D. 

sudo apt update

sudo apt install -y build-essential libc6-dev

- [cpp 11](https://github.com/engineer-e/WSL-Jupyter-Kernel/blob/main/check_cpp_11.ipynb)
- [cpp 14](https://github.com/engineer-e/WSL-Jupyter-Kernel/blob/main/check_cpp_14.ipynb)
- [cpp 14](https://github.com/engineer-e/WSL-Jupyter-Kernel/blob/main/check_cpp_17.ipynb)

![alt text](kernel/cpp_kernel.png)

# Super!!! - Successfully Completed (^o^)


