---
layout: post
title: "Grep and Regex in Practice"
date: "2020-01-12"
last_modified_at: null
pin: false
---

Much like yesterday, this was a fairly quick session. The weekends seem to get away from me and I need to get better at managing my time if I want to progress through these courses. Today I worked through the practicals for *3.2. Searching and Extracting Data from Files*.

- `ls <directory> | wc -l`: The `ls` command outputs the files and folders within a given directory into the pipe (`|`). From the pipe, we can count the number of files with `wc` and the `-l` option (which prints the newline counts) to determine the amount of files/folders in the directory.

- `cat <file> | grep <phrase> | wc -l`: Used to determine how often a given phrase appears in a file. The `grep` command searches for the phrase and pipes it into the `wc -l` command to count how many times it appears.

- `cat <file> | grep -E "^<character>" | wc -l`: Counts how many words begin with a certain character in a given file. the `-E` option after the `grep` command denotes that the pattern following will be regex. The carat symbol (^) matches the start of the string with the given character.

- `cat <file> | grep -E "^<character 1>...<character 2>$"`: Used to search for a word that begins with character 1, ends with character 2, and is 5 characters long in total. The "5 characters in total" is specified by the three dots plus the two other character expressions.

- `cat <file> | grep -E "^<character 1>..$|^<character 2>..$" | wc -l`: Used to count how many three letter words start with character 1 OR character 2. It is important to note that the 'pipe' symbol within the regex is an OR operator.