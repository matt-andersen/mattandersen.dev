---
layout: post
title: "Free as in Freedom"
date: "2020-01-09"
last_modified_at: null
pin: false
---

I finally sorted out my subscription for Linux Academy, so I went back and finished up _Source Control with Git_. Which means another course ticked off my list.

As mentioned yesterday, I have reshaped the direction of my learning. I have decided to replace my previous course list with the [Junior DevOps Learning Path](https://linuxacademy.com/learning-path/junior-devops-engineer-entry-level/) provided by Linux Academy. This will give me some needed structure for my learning. The [LPI Linux Essentials Certification](https://linuxacademy.com/cp/modules/view/id/346) course is recommended before taking this learning path. So, this is the course I started on today. Below are a few notes:

- `ls -a` or `ls --all`: Allows you to see all files in a directory, even hidden files. Hidden files in Linux are denoted by a dot (such as .gitignore).

- `ls -l`: Refers to the 'long listing'. Includes file ownership and permissions.

- `ls -s`: Shows file size information.

- `ls -h`: Provides size in a human readable format. For example, it shows 4 kilobytes as 4K instead of 4096. Must be used in conjunction with the `-s` option to work, such as `ls -sh`.

- `ll`: An alias for `ls -l`. Varies per each Linux distribution.

- `$PS1`: Refers to the primary prompt string. The prompt refers to the string in the shell prior to the cursor, for example `[matt@localhost ~]$`. The \$PS1 variable is the format of this string. An example format is `[\u@\h \W]\$` where each of those characters pertains to a value in the string above.

- Variables can be used to store the output from certain commands. If a variable such as `var1=$(ls)` is set. Every time `echo $var1` is executed, the `ls` command will be run and files in the directory will be displayed in the terminal.

- Quoting:
  - Escape character (\\\): will preserve the value of the _next following_ character.
  
  - Single quotes: will preserve the literal value of _every_ character contained within the quotes. Including the escape character.
  
  - Double quotes: will preserve the value of _most_ characters except for \$, single quotes, and the escape character.
