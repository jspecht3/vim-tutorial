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
This section will cover the most bare-bones usage of vim. With this, you will be able make a file, move around inside that file, and save the file, but not much else. You should be able to finish this section in less than 5 minutes.

To begin, we are going to create a text file named `example.txt`. We can do this one of two ways: using `touch` to create a file then opening it with `vi` / `vim` or using `vi` / `vim` to create a file and open that file in a single command.
```
# method 1: creating a file with touch
$ touch example.txt
$ vi example.txt

# method 2: creating a file with vi
$ vi example.txt
```

You should see a screen that looks like the one below.
---insert the image of the opening vim screen

By default, you are in "normal" mode. In normal mode, you cannot type. To begin typing, you need to hit :sparkles: `i`, which puts you into "insert" mode. You will know you are in insert mode with a flag at the bottom of the terminal as below.
---insert the image of the insert mode

Once in insert mode, you can begin typing like usual. Let's type some example text. 
```
This is some example text.
```

If you want to go to a new line, you can use :sparkles: `enter` as expected. Let's create another line with some more text.
```
This is some example text.
You get another line when hitting enter.
```

Now that we have some text, let's navigate around and edit some text. After typing, your location in the text (indicated by the flashing white box) should be at the end of the file.
---insert the image of the end of text.

We can navigate between lines using the :sparkles: the `up arrow` key to move up a line and the :sparkles: the `down arrow` key to move down a line. Similarly, we can navigate inside of a line by using :sparkles: the `left arrow` key to move left and :sparkles: the `right arrow` key to move right. Using the arrow keys, navigate in the file so your cursor is in the same spot as mine.
---cursor at example

Notice the cursor over the "e" in example. :red_circle: When entering text, you will insert the text **before** the cursor. In this case, we any text we enter will go after "This is some " and shift "example text." to the right.

Let's add some more text into the first line.
```
This is some more or additional example text.
You get another line when hitting enter.
```

Rereading this sentence, it seems somewhat repetitive. Let's remove " or additional" to make the sentence more concise. We can remove text with :sparkles: the `backspace` key as per usual. After the change, your text file should read as follows.
```
This is some more example text.
You get another line when hitting enter.
```

After these revisions, we are ready to save the file. To save, we need to get back into normal mode by using :sparkles: the `esc` key. Once we are back in normal mode, the "-- INSERT --" at the bottom of the screen will have gone away.

:red_circle: To determine which mode you are in, look at the bottom of the screen. If there is no indicator, you are in normal mode. If there is an indicator, it will tell you what mode you are in.

Now that we are in normal mode, we want to save and close the file. To do this, we first hit :sparkles: `:`, which shows at the bottom of the sreen and indicates you want to enter certain commands.
---colon

After entering this "command" mode. We can save the changes we have made and close the file by typing :sparkles: `wq` after the `:` and then hitting enter.
---wq

Here, `wq` stands for "write" and "quit", which saves the changes made to the file and closes it aswell.

You can also execute these commands independently. For example, you can use `:w` if you want to save your work, but still continue editing the file. Also, if you want to quit a file without making any changes, you can use `:q`.

:red_circle: If you are ever lost while using vim, you can usually regain your bearings by hitting the `esc` key a few times to return to normal mode.

With this, you now have the basic framework to create, navigate, and edit files using vim.
