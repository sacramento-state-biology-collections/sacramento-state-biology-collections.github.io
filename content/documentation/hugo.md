---
title: "Hugo Manual"
date: 2022-10-14T16:14:58-07:00
draft: false

---

## Installing Hugo on your System

### For Windows

#### Step 1: Install Scoop onto your system

Open Windows Powershell and enter these commands:

>Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

(If you get a message about an Execution Policy Change, press y then hit enter).

>irm get.scoop.sh | iex

#### Step 2: Install Hugo with Scoop

>scoop install hugo

Hugo is now Installed!

### For MacOS

#### Step 1: Install Homebrew onto your system

Open the macOS Terminal and enter:

>/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

#### Step 2: Install Hugo with Homebrew

>brew install hugo

Hugo is now installed!

## Running the Hugo Server 