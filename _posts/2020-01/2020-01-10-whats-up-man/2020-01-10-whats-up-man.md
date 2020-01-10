---
layout: post
title: "What's Up Man?"
date: "2020-01-10"
last_modified_at: null
pin: false
---

I just realised, yesterday marked a 7-day streak of making at least one commit per day! Which is currently the longest streak on my GitHub profile.

Today I am back on the _LPI Linux Essentials Certification_ course. I am not sure whether I will take the certification course itself, but this is something I'll look into in the future. Today was pretty content heavy and I got to meet my new friend, "man". I omitted some notes from this post since it was getting a bit long:

- View release information:

  - `lsb_release -a`: Shows the current distro, version, and release number.

  - `cat /etc/*release*`: Used to display release files. The asterisks make use of a feature called _globbing_ which searches for every file containing "release". More on globbing [here](https://linuxhint.com/bash_globbing_tutorial/).

- User information:

  - `w`: Displays all users currently logged in.

  - `last`: Shows the last user who logged in and when the system was last booted.

  - `>` & `>>`: The angle brackets can be used to add contents to a file. The single bracket writes to a file, either by creating a file or overwriting a previous file. Whilst the double brackets append to the end of an existing or new file. For example, `w >> log.txt` would append a list of users currently logged-in to a file called log.txt.

- Man pages and Info pages:

  - Manual pages (man pages) of commands can be opened by writing `man <command>` for example `man ls`.

  - Whilst a man page is open, entering a forward slash and typing in a phrase will highlight where that phrase appears in the man page.

  - Using `n` and `N` allows you to traverse through these highlighted phrases in descending and ascending order respectively.

  - Info pages are Invoked via `info <command>`. They are similar to man pages but more in-depth. If an info page can't be found, then the command will just show the man page - this is common for third-party packages.

- Files and directories:

  - Change directory:

    - Just typing `cd` will take you to the home directory.

    - `cd /`: Changes the directory to the root level. Similar to C: in Windows.

    - `cd -`: Goes back to previous directory.

  - [This link](https://www.howtogeek.com/117435/htg-explains-the-linux-directory-structure-explained/) explains the folders that make up the Linux root directory.

  - Display directory contents:

    - `ls -t`: Sort by file date, in order of newest to oldest.

    - `ls -S`: Sort by file size, largest to smallest.

    - `ls -u`: Display when the file was last accessed. Needs to be used in conjunction with the `-l` (long listing) option.'

  - More file & directory commands:

    - `cp <source> <destination>`: Used to copy files and folders. The `-r` (recursive) option needs to be added to copy folders.

    - `mv <source> <destination>`: Used to move files/folders as well as rename them.

    - `file`: Displays the type of the file
