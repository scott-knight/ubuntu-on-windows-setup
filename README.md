# ubuntu-on-windows-setup
This content used to help setup Ubuntu on Windows 10, to semi-replicate a Mac terminal setup for developing Ruby on Rails (or any other code you would want to use).

I use this for my own purposes, but you, the reader, can use this information for your own purposes as well. These instructions are given only for demonstration purposes, they are not a definitive guide on how to setup a Windows 10 to use Ubuntu or any other content. Follow the instructions at your own risk. You bear the full responsibility of the outcome for following these instructions. By using these instructions, you agree to owning and accepting the full liablity of the outcome or result. Additionally, you are welcome to fork this project/information and/or submit pull requests (PR) to add to the information of the project. I retain the right to accept or reject any PR for any reason. You are welcome to write up your own doc and post it where you want if you don't agree with what's posted. Now that we understand what this is for, let's move on to the good parts.

Below is the step-by-step guide on how to install all the bits needed to get an Ubuntu instance installed, setup and customized to a state where you can use a console session to write and push code. The details of each of the steps (and there precise order of install) are a little hazy as I went through this process over the course of a few days. Additionally, I didn't anticipate creating a step-by-step guide, but I found myself creating notes incase I blew my Windows 10 install (which never happened) and/or my Ubuntu install (which I did happen several times). That being said, here is the (fuzzy) list of things that need to be done in order to get things working.

1. [Install WSL2](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-wsl2.md)
2. [Install VSCode (if you want)](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-vscode.md)
3. [Install Windows Terminal](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-windows-terminal.md)
4. [Install oh-my-posh and required libraries](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/Install%20oh-my-posh-and-required-libraries.md)
5. [Install Ubuntu](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-ubuntu.md)
6. [Configure Windows Terminal](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/configure-windows-terminal.md)
7. [Configure Ubuntu](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/configure-ubuntu.md)

Once you have completed steps 1-4, you shouldn't have to do them again. Once Windows Terminal is setup, you should be good for the lifetime of your Windows 10 install (pending needed updates if there are any).

You will need to repeat steps 5-7 if you decide to delete your current install of Ubuntu and reinstall it.

<br/>

## Install WSL2

This is required to install the Windows Subsystem which runs virtual instances on Windows. Instructions to install WSL2 can be [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-wsl2.md).


## Install VSCode

You DON'T actually have to do this if you prefer using VIM or Nano to edit config files or write code. I prefer using it, therefore recommend installing it. One of the great features of VSCode is the ability to save/sync your VSCode settings to Github. More details can be found in the [install doc](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-vscode.md).

<br/>

## Install Windows Terminal

To get everything working correctly, you will need to install the new Windows Terminal as it IS NOT installed by default. Install instructions for installing Windows Terminal can be [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-windows-terminal.md).

<br/>

## Install oh-my-posh and Required Libraries

[Oh-my-posh](https://ohmyposh.dev/) is akin to [oh-my-zsh](https://ohmyz.sh/), but is for the Windows PowerShell which is used in the Windows Terminal. [On the main page](https://ohmyposh.dev/), it says it can be used in any shell. [In other documentation](https://docs.microsoft.com/en-us/windows/terminal/tutorials/powerline-setup#set-cascadia-code-pl-as-your-font) it outlines how to set this up for PowerShell and the Ubuntu instance.

There's a small amount of setup needed to get everything inline for running (my personal preference for) zsh instances. You don't have to do this step either if you don't plan on using a powershell or zsh theme which requires Powerline icons. Documentation for this install is [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/Install%20oh-my-posh-and-required-libraries.md).

<br/>

## Install Ubuntu

This is the simplest step. Documentation is [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-ubuntu.md).

<br/>

## Configure Windows Terminal

Once you have Ubuntu installed you will need to configure Windows Terminal to use the correct fonts which contain the Powerline icons. Again, you don't have to do this step if you aren't using Windows Terminal powershell or a zsh theme that don't require them. I use themes that use the icons. I beleive it makes it eaiser to read and give the conosle a great appearance. Instructions for configuring Windows Terminal can be [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/configure-windows-terminal.md).

<br/>

## Configure Ubuntu

This is the step-by-step guide for setting up Ubuntu to use all the settings, aliases, functions, etc. that I use every day. You don't have to do this step either. Ubuntu runs with or without this customization. Also, if you go through the step-by-step guide and don't like the setup, you can simply delete the Ubuntu instance and reinstall it. It will be a completely clean install of Ubuntu, no settings will carry over. Configuration instructions can be [found here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/configure-ubuntu.md).
