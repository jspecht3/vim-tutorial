# vim-tutorial
Tutorial for vim geared towards complete beginners. With this, you should be able to comptently use vim in the terminal.

Like everything in life, when first learning something new, try establishing a basic framework you can later integrate more complexity. To develop this framework, you can go to [Absolute Basics](#absolute-basics).

Before you start the tutorial, make sure you have vim installed using `vi --version | head -1`. You should see that you have VIM - Vi IMproved like below. If you do not see this, search on the internet "how to install vim on <your-operating-system>" (if you are using wsl, make sure to choose the linux distro your subsystem is running).
```
$ vi --version | head -1
VIM - Vi IMproved 9.1 (2024 Jan 02, compiled May 03 2024 02:45:42)
```

The first time a command is used in the tutorial, a ✨ will be placed in front of that command. Important concepts will be marked with a 🔴.

# List of Commands


# Absolute Basics
This section will cover the most bare-bones usage of vim. With this, you will be able make a file, move around inside that file, and save the file, but not much else. You should be able to finish this section in less than 3 minutes.

To begin, we are going to create a text file named `example.txt`. We can do this one of two ways: using `touch` to create a file then opening it with `vi` / `vim` or using `vi` / `vim` to create a file and open that file in a single command.
```
# method 1: creating a file with touch
$ touch example.txt
$ vi example.txt

# method 2: creating a file with vi
$ vi example.txt
```









