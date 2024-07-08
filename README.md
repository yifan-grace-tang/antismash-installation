# antiSMASH Installation Guide

<img src="https://antismash.secondarymetabolites.org/images/antismash_logo.svg" height="200">

__Please read through this entire guide before getting started as it will save you a lot of time troubleshooting errors later on__. 

Even if you have never installed similar softwares on your computer before, you should be able to install antiSMASH _as long as you read this guide thoroughly_.

## Before You Get Started

- Unless otherwise specified, use the copy button feature on GitHub __ONLY__, do not attempt to manually type commands into your terminal.

- If commands are expected to take a long time to complete they will be indicated with this icon ⌛. This means that either you should wait until a confirmation/continue action or wait until you can type again. You should see something like this when you are able to type again:

__For Macbook Pro__
```
(base) username@your-mbp ~ % |
```
__For Macbook Air__
```
(base) username@your-air ~ % |
```

__For a Windows Computer (Powershell)__
```
PS C:\Users\username> |
```

__For a Windows Computer (Ubuntu)__
```
(base) username@Name:~$ |
```

- When editing text in the terminal window you __cannot highlight__ a particular area __and delete__ with your keyboard. Instead to delete a portion of your command you must use your left arrow and navigate to the portion you want to edit

## Installation Steps

>[!IMPORTANT]
> If you have installed BiG-SCAPE as detailed in [these instructions](https://github.com/yifan-grace-tang/bigscape-installation/blob/main/README.md) then you can skip straight to __antiSMASH Installation__ for your respective platform

Follow the links for your platform __do not use Windows instructions for Mac or vice-versa__. These steps are _dependent on each other_ so follow them sequentially.

For __Mac__:

1. [🐍 Miniconda Installation](#-miniconda-installation-mac)
2. [🌱 antiSMASH Installation](#-antismash-installation-mac)

For __Windows__:

1. [🐧 WSL Installation](#-wsl-installation-windows)
2. [🐍 Miniconda Installation](#-miniconda-installation-windows)
3. [🌱 antiSMASH Installation](#-antismash-installation-windows)

# Mac Based Installation

Follow these instructions __only__ if you are using a Mac. The expectation is that you first do `conda` installation, then `antismash` installation.

## 🐍 Miniconda Installation (Mac)

> [!WARNING]  
> __Follow the file download instructions very carefully! If you don't download the right file, there will be lots of troubleshooting.__

> [!NOTE]
> Miniconda is also refered to as `conda` and those terms will be used interchangibly in this installation guide.

1) Check if conda is already installed on your computer. Paste in your `terminal` <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b3/Terminalicon2.png/240px-Terminalicon2.png" width="20" height="20" align="center"/> :

```bash
conda -V
```

2) If the `conda` is already installed, you will see a message similar to the one below (versions can differ). Proceed to the [antiSMASH Installation](-antismash-installation-mac) section.

```bash
conda 24.5.0
```

3) If the `conda` is __not__ installed, then you will see the message below - proceed to step 4:

```bash
zsh: command not found: conda
```

4) Navigate to [this link](https://docs.anaconda.com/miniconda/#latest-miniconda-installer-links) and download the installer version as specificied in the images __DO NOT SELECT ANY OTHER INSTALLER__. Click the link under the _Name_ field to begin installation

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/correct-miniconda-install.png" height="500">
</p>
   

5) Open a new `terminal` window and copy-paste the command below:

```bash
cd downloads
```
 
6) ⌛ Paste into your terminal:

```bash
bash Miniconda3-latest-MacOSX-x86_64.sh
```

7) You will now be prompted for a series of agreements that you must accept from your terminal. These are included below:

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/conda-64bit-accept-small.png" height="99">
  <br>
  <em>Here type the word 'yes' and click enter </em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/conda-tos.png" height="283">
  <br>
  <em>When you see the Terms of Service (TOS) use your down arrow key to get through the text</em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/conda-tos-accept.png" height="107">
   <br>
  <em>After you finish scrolling through the TOS type the word 'yes' to move on</em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/conda-install-accept-small.png" height="146">
   <br>
  <em>Complete the installation by clicking the 'return' key</em>  
</p>

8) Close your `terminal` window and open a __new__ `terminal` window.

9) Check if conda is successfully installed on your computer. Paste in your `terminal`:

```bash
conda -V
```

10) If the `conda` is sucessfully installed, you will see a message similar to the one below (versions can differ). Proceed to the [antiSMASH Installation](-antismash-installation-mac) section.

```bash
conda 24.5.0
```

## 	🌱 antiSMASH Installation (Mac)

`todo`

# Windows Based Installation

Follow these instructions __only__ if you are using a Windows machine. The expectation is that you first do `wsl` installation, then `conda` installation, then `antismash` installation.

## 🐧 WSL Installation (Windows)

1) Check if `wsl` is already installed on your computer. Look through your applications and see if there is an  `ubuntu` <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/UbuntuCoF.svg/1024px-UbuntuCoF.svg.png" width="20" height="20" align="center"/> application on your machine.

2) If you see `ubuntu` on your machine proceed to the [Miniconda Installation](#-miniconda-installation-windows) section.

3) If you cannot find the `ubuntu` application proceed to step 4.

4) Find your __Windows PowerShell__ <img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/PowerShell_5.0_icon.png" width="20" height="20" align="center"/> application and _run as administrator_. You will be asked to confirm if you "want to allow this app to make changes to your device" - click yes.

5) ⌛ Paste into your `powershell`:

```bash
wsl --install
```

6) Restart your computer for the changes to activate.

7) After your computer restarts, the `ubuntu` application should now be available, open this app:

8) The first time you open this app you will be prompted to create a username and password. _This is in no way tied to your Windows account so choose whatever you would like_. This input will look like below:

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/wsl.png" height=130> 
  <br>
  <em>Type username, click enter, type password, click enter, retype password, click enter.</em>
</p>

> [!WARNING]  
> Note down the password that you create, it will be used later on.

> [!NOTE]
> You will not be able to see the password you type, so just type your password and click enter.

9) After you create your username and password you can now close the `ubuntu` app and proceed to [Miniconda Installation](#-miniconda-installation-windows)

## 🐍 Miniconda Installation (Windows)

> [!WARNING]  
> __Follow the file download instructions very carefully! If you don't download the right file, there will be lots of troubleshooting.__

> [!NOTE]
> Miniconda is also refered to as `conda` and those terms will be used interchangibly in this installation guide.

1) Check if conda is already installed on your computer. Paste in your `ubuntu` <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/UbuntuCoF.svg/1024px-UbuntuCoF.svg.png" width="20" height="20" align="center"/> :

```bash
conda -V
```

2) If the `conda` is already installed, you will see a message similar to the one below (versions can differ). Proceed to the [antiSMASH Installation](-antismash-installation-windows) section.

```bash
conda 24.5.0
```

3) If the `conda` is __not__ installed, then you will see the message below - proceed to step 4:

```bash
conda: command not found
```

4) Navigate to [this link](https://docs.anaconda.com/miniconda/#latest-miniconda-installer-links) and download the installer version as specificied in the images __DO NOT SELECT ANY OTHER INSTALLER__. Click the link under the _Name_ field to begin installation

<p align="center">
  <img src="./img/miniconda_wsl_install.png" height="300">
</p>
   

5) Open a new `ubuntu` window and copy-paste the command below. Replace __USERNAME__ with your Windows username:

```bash
cd ../../mnt/c/Users/USERNAME/Downloads
```

> [!NOTE]
> To find your __USERNAME__ you can open the `powershell` <img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/PowerShell_5.0_icon.png" width="20" height="20" align="center"/> application and type the command `$ENV:UserName` and click enter. Copy the value that you see.
 
6) ⌛ Paste into your ubuntu:

```bash
bash Miniconda3-latest-Linux-x86_64.sh
```

7) You will now be prompted for a series of agreements that you must accept from your terminal. These are included below:

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/miniconda_windows_license.png" height="99">
  <br>
  <em>Here click enter </em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/miniconda_windows_lic_scroll.png" height="150">
  <br>
  <em>When you see the Terms of Service (TOS) use your down arrow key to get through the text</em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/miniconda_lic_final.png" height="110">
   <br>
  <em>After you finish scrolling through the TOS type the word 'yes' to move on</em>
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/miniconda_install_accept.png" height="183">
   <br>
  <em>Confirm the installation by clicking the 'return' key</em>  
</p>

<p align="center">
  <img src="https://github.com/yifan-grace-tang/bigscape-installation/blob/main/img/conda_windows_accept_final.png" height="85">
   <br>
  <em>Finalize the installation by typing 'yes' and clicking enter</em>  
</p>


8) Close your `ubuntu` window and open a __new__ `ubuntu` window.

9) Check if conda is successfully installed on your computer. Paste in your `ubuntu`:

```bash
conda -V
```

10) If the `conda` is sucessfully installed, you will see a message similar to the one below (versions can differ). Proceed to the [antiSMASH Installation](-antismash-installation-windows) section.

```bash
conda 24.5.0
```

## 	🌱 antiSMASH Installation (Windows)

`todo`
