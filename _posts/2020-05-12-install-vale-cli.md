---
layout: post
title: "Vale Series: How to install the Vale CLI (1/3)"
author: deanna
comments: true
---

In this tutorial, you'll learn how to install Vale, a style linter. This tool allows you to lint your doc files. This is the first in a three-part series about using Vale.

## Assumptions

You have some familiarity with using the command line. If you're a Mac user, keep on reading. If you're working on Windows, click [here](#instructions-for-windows-users).

## Instructions for Mac users

To install Vale on your computer, you'll need to use a package manager. Package managers allow you to install and update packages and libraries.

The best package manager for macOS is [**Homebrew**][Homebrew link]. If you've already installed Homebrew, skip to step two. Otherwise, continue reading the instructions below.


## Step one: Install Homebrew

1. To install Homebrew, enter this command into the terminal (feel free to copy and paste): `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

2. To verify that you installed Homebrew, run the command `brew help`. If the installation was successful, the command prints the help documentation to the terminal.

## Step two: Install Vale

1. From the terminal, run the command `brew install vale`. You'll see some output in the terminal as Homebrew installs Vale.

2. Verify that the `vale` command is now available by running `vale -v` in the terminal. If the installation was successful, the command reports the latest, stable version of Vale.

---

## Instructions for Windows users

To install Vale on your computer, you'll need to use a package manager. Package managers allow you to install and update packages and libraries.

Windows users can install Vale using [**Chocolatey**][Chocolatey link]. If you've already installed Chocolatey, skip to step two. Otherwise, continue reading the instructions below.

---

## Step one: Install Chocolatey

1. Follow [these](https://chocolatey.org/install) steps to install Chocolatey on your computer.

2. To verify that you installed Chocolatey, run the command `choco -?`. If the installation was successful, the command prints the help documentation to the terminal.

## Step two: Install Vale

1. From the terminal, run the command `choco install vale`. You'll see some output in the terminal as Chocolatey installs Vale on your computer.

2. To verify that you installed Vale, run the command `vale -v` in the terminal. If the installation was successful, the command reports the latest, stable version of Vale.

---

That's all you need to do to install the Vale CLI! Next, you'll learn how to configure and customize Vale for your documentation needs.

[Chocolatey link]: https://package.chocolatey.org/

[Homebrew link]: https://brew.sh/



