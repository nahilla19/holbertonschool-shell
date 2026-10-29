# Shell permissions

This directory contains scripts for practicing Linux user and file permissions.

## 0. My name is Betty

`0-iam_betty` switches the current user to `betty` using `su betty`.

## 1. Who am I

`1-who_am_i` prints the effective username of the current user using `whoami`.

## 2. Groups

`2-groups` prints all groups the current user belongs to using `groups`.

## 3. New owner

`3-new_owner` changes the owner of the file `hello` to the user `betty` using `chown betty hello`.

## 4. Empty!

`4-empty` creates an empty file named `hello` using `touch hello`.

## 5. Execute

`5-execute` adds execute permission to the owner of `hello` using `chmod u+x hello`.

## 6. Multiple permissions

`6-multiple_permissions` adds execute permission to the owner and group, and read permission to others on `hello` using `chmod ug+x,o+r hello`.

## 7. Everybody!

`7-everybody` adds execute permission for the owner, group, and others on `hello` using `chmod a+x hello`.

## 8. James Bond

`8-James_Bond` removes all permissions from the owner and group, and grants read, write, and execute permissions to others on `hello` using `chmod 007 hello`.

## 9. John Doe

`9-John_Doe` sets the permissions of `hello` to `-rwxr-x-wx` using `chmod 753 hello`.

## 10. Look in the mirror

`10-mirror_permissions` copies the permissions of `olleh` to `hello` using `chmod --reference=olleh hello`.

## 11. Directories

`11-directories_permissions` adds execute permission for the owner, group, and others to every immediate subdirectory of the current directory, without changing regular files, using `find . -mindepth 1 -maxdepth 1 -type d -exec chmod a+x {} +`.

## 12. More directories

`12-directory_permissions` creates a directory named `my_dir` with permissions `751` using `mkdir -m 751 my_dir`.

## 13. Change group

`13-change_group` changes the group owner of the file `hello` to `school` using `chgrp school hello`.
