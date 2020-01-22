---
layout: post
title: "Sudo Make Me a Sandwich"
date: "2020-01-21"
last_modified_at: null
pin: false
---

The [inspiration behind my title](https://xkcd.com/149/) and also [another good and relevant xkcd](https://xkcd.com/838/).

It's been some time since I last made a post. I haven't done any Linux Academy courses since, but I have been doing a bit of coding in Python. Today I finished the LPI Essentials Linux Course. Reflecting on what I have learnt in this course, Linux now feels more demystified. Also, my confidence in using the terminal has definitely risen.

In future, I am thinking of breaking up larger posts into several smaller ones. As opposed to having one big daily post. 

- Using sudo:

  - `su`: Sets a superuser.

  - `/etc/sudoers`: Contains various rules pertaining to what users have what types of sudo access.

  - `sudo su -`: Switches to root user.

- Handling groups:

  - `groups <username>`: Displays a list of groups a user is a part of.

  - `cat /etc/passwd | grep <username>`: Shows the users home directory, ID, and login shell.

  - `useradd <username>`: Creates a new user with the designated username.

  - `sudo passwd <username>`: Elevates privileges to set a password for a given user.

  - `/etc/skel`: Stores files that are automatically added to a new user's home directory.

  - `groupadd <groupname>`: Creates a new group.

  - `for i in <username1> <username2>; do sudo usermod -a -G <groupname> $i; done`: Allows you to add multiple users to a certain group at once.

  - `passwd -l <username>`: Locks a user account.

- File and directory permissions:

  - `chown <user><:group> <file>`: Changes the user and/or group ownership of a given file.

  - `chmod <permissions> <filename>`: Modifies the permissions (read, write, execute) for a file.

- Temp files & symbolic links:

  - `mktemp`: Makes a temp file with a random name located at /tmp/.

  - `ln -s <file> <linkname>`: Creates a link to a specified file.
