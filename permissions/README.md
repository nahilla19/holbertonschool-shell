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
