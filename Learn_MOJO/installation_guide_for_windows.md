# Installing and Using Mojo Programming Language on Windows

## Introduction

Mojo is a powerful and efficient programming language that combines the usability of Python with the performance of C, unlocking unparalleled programmability of AI hardware and extensibility of AI models.

## Installation

As of now, Mojo is not available for Windows directly. However, you can use it on a Linux container or remote system. Here's how you can do that with Windows Subsystem for Linux (WSL):

1. **Enable WSL**: First, you need to enable the WSL feature on Windows. You can do this by opening PowerShell as Administrator and running the command 
    ```bash
    wsl --install
    ```
    This will automatically enable the necessary optional components, download and install the latest Linux kernel, set WSL 2 as your default, and install a Linux distribution for you.

2. **Install Linux Distro**: Install a Linux distribution using WSL. Ubuntu 22.04 is recommended. You can install it from the Microsoft Store.

3. **Set Ubuntu to use WSL 2**: Set your Ubuntu to use WSL 2. You can do this by opening PowerShell and running the command 
    ```bash
    wsl --set-version Ubuntu-22.04 2
    ```

4. **Check WSL Version**: Check the version of WSL and update it if necessary. You can check your WSL version by opening PowerShell and running the command 
    ```bash
    wsl --list --verbose
    ```

## Setting Up Development Environment

1. **Install VS Code**: Install Visual Studio Code, which is a popular code editor. You can download it from the official website and follow the installation instructions.

2. **Install WSL Extension**: Install the WSL extension for VS Code. This extension lets you use the Windows Subsystem for Linux as your full-time development environment right from VS Code.

3. **Install Mojo Extension**: Install the Mojo extension for VS Code. This extension provides support for Mojo programming language in Visual Studio Code.

## Installing Mojo

1. **Install Modular CLI**: The Mojo SDK is available through the Modular CLI tool, which works like a package manager to install and update Mojo. You can install it by running 
    ```bash
    npm install -g modular-cli
    ``` 
    in your terminal.

2. **Install Mojo**: Use the Modular CLI to install Mojo. You can do this by running 
    ```bash
    modular add mojo
    ```
    in your terminal.

## Using Mojo

1. **Create Your First Program**: Once you have installed Mojo, you can start writing your first program. Open VS Code, create a new file with a `.mojo` extension, and write your program.

2. **Save and Run Your Program**: After writing your program, save it with a `.mojo` extension and run it. You can run your program by opening a terminal in VS Code (View > Terminal), navigating to your file's directory, and running `mojo run filename.mojo`.

## Conclusion

That's it! You have successfully installed and set up Mojo on your Windows machine using WSL. Now you're ready to start exploring this powerful programming language!
