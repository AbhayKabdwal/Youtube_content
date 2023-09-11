# How to Install Git on macOS

## Step 1: Open Terminal
You can find the Terminal application through Spotlight Search or it is usually located in the Utilities folder which is in the Applications folder.

## Step 2: Check if Git is Already Installed
Git comes pre-installed on most versions of Mac, and there's a chance you already have it. In your terminal, type `git --version`.

```bash
git --version
```

If Git is installed, you’ll see a message with the installed version. If not, you’ll see a prompt to install it.

## Step 3: Install Git with Homebrew

If Git is not installed, the easiest way to install it is by using Homebrew. If you don’t have Homebrew installed, you can install it by pasting the following command in your terminal:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once Homebrew is installed, you can install Git by typing:
```bash
brew install git
```

## Step 4: Verify Installation

After the installation is complete, verify it by checking the Git version:
```bash
git --version
```


You should now see the installed version of Git.