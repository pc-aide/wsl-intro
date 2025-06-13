# Understanding WSL (Windows Subsystem for Linux)

## Overview

**WSL (Windows Subsystem for Linux)** allows you to run a full Linux environment directly on Windows without the need for a dual-boot setup or a traditional virtual machine. It is ideal for developers, system administrators, and students who want to use Linux tools and workflows on a Windows PC.

## Key Features

- Run native Linux command-line tools (bash, ssh, git, etc.) on Windows.
- Access Windows files from Linux and vice versa.
- Support for multiple Linux distributions (Ubuntu, Debian, Kali, etc.).
- Integration with Windows tools like PowerShell and VS Code.
- WSL 2 includes a full Linux kernel with improved performance and compatibility.

## WSL vs WSL 2

| Feature                 | WSL 1                       | WSL 2                        |
|------------------------|-----------------------------|------------------------------|
| Kernel Type            | Translation layer           | Full Linux kernel (via VM)   |
| Performance (I/O)      | Slower                      | Faster file system access    |
| Compatibility          | Limited                     | Full system call support     |
| File System            | Uses Windows file system    | Uses virtual disk (.vhdx)    |

## Getting Started

### 1. Prerequisites

- Windows 10 version 2004 or higher (Build 19041+), or Windows 11

### 2. Installation Steps (WSL 2)

Open PowerShell as Administrator and run:

```powershell
wsl --install
