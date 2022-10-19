---
title: "Hugo Manual"
date: 2022-10-14T16:14:58-07:00
draft: false

---

## What is Hugo?

Hugo is a static site generator we are using to display project information on a website viewable by anyone. We are using a custom theme called Mainroad.

## Installing Hugo on your System

### For Windows

#### Step 1: Install Scoop onto your system

Open Windows Powershell and enter these commands:

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

(If you get a message about an Execution Policy Change, press y then hit enter).

```powershell
irm get.scoop.sh | iex
```

#### Step 2: Install Hugo with Scoop

```Powershell
scoop install hugo
```

Hugo is now installed! You'll need to restart your system for it to work.

### For MacOS

#### Step 1: Install Homebrew onto your system

Open the macOS Terminal and enter:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Step 2: Install Hugo with Homebrew

```bash
brew install hugo
```

Hugo is now installed! You'll need to restart your system for it to work.

## Running the Hugo Server 

1. Open up the project in Visual Studio Code

2. Open the terminal
3. Make sure the terminal is in `sacramento-state-biology-collections.github.io` Directory
4. Enter this command in the terminal: hugo server
5. If the terminal says the web server is available, then that means it worked!
6. Whenever you want to stop running the server, press ctrl + c in the terminal

## Viewing the Hugo Page in VS Code While Editing the Project Code

1. After the server starts running, it will tell you what address the web server is available at. An example is **http://localhost:1313/**. Copy this address to your clipboard

2. Press `ctrl + p` to open the VS Code search bar
3. Enter: `>Simple Browser: Show`
4. Paste the address you copied in step 1 into the simple browser's search bar
5. Drag it to the right side of VS Code to display the site to the right and your code on the left
6. Now everytime you make a change to the code and save, you will see the website update in real time!

#### If the site isn't displaying properly, try these steps.

1. Stop the server by pressing ctrl + c in the terminal

2. Delete the Mainroad folder
3. Enter this command in the terminal: 
    - `git submodule add -f https://github.com/vimux/mainroad.git themes/mainroad`
4. Run the server again

## Creating New Pages

1. Open a second terminal in VS Code. Don't close the one that's running the server.

2. Type the command: `hugo new (folder you want the file in)/filename.md`. For example, if you wanted to create a file named hugo in the documentation folder, you would enter: `hugo new documentation/hugo.md`
3. The top will have a title, date, and draft. You need to change `draft: true` to `draft: false` for the page to appear on the website.
4. You should now have a brand new page!

## Links for More Information

- [Hugo Documention](https://gohugo.io/documentation/)
- [Mainroad Documentation](https://mainroad-demo.netlify.app/docs/)