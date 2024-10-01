# Stable-ts Deployment Guide

This guide will walk you through the deployment of Stable-ts on a Windows system. It includes instructions for setting up the necessary prerequisites, creating a virtual environment, and installing Stable-ts.

## Prerequisites

### 1. FFmpeg

Stable-ts requires FFmpeg to be installed and available in the system PATH. You can install FFmpeg using one of the following methods:

#### **Windows using Chocolatey**
```bash
choco install ffmpeg
```

#### **Windows using Scoop**
```bash
scoop install ffmpeg
```

### 2. Pytorch

Stable-ts requires PyTorch, preferably with GPU support for optimal performance. Install the GPU version of PyTorch using the following command:
```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

## Setting Up the Virtual Environment

- Open a terminal (Command Prompt or PowerShell).
- Navigate to your project directory.
- Create a new virtual environment using the following command:
  ```bash
  python -m venv stable-ts-env
  ```
- Activate the virtual environment:
  ```bash
  stable-ts-env\Scripts\activate
  ```

## Installing Stable-ts

With the virtual environment activated, install Stable-ts:

- Install the stable release:
  ```bash
  pip install -U stable-ts
  ```
- Install the latest repository:
  ```bash
  pip install -U git+https://github.com/jianfch/stable-ts.git
  ```
## Verification

After installation, verify that Stable-ts is correctly installed by running:
```bash
stable-ts --help
```
If the command returns a help message, your setup is complete.
  
