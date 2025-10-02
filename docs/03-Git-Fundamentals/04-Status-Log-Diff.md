---
title: Status, Log, and Diff
layout: default
parent: Git Fundamentals 
nav_order: 4
---

<!-- prettier-ignore-start -->
# Status, Log, and Diff
{: .no_toc }

Status, Log, and Diff are all git commands that help the user manage their projects. Status allows the user to check the status of their repo. Log allows the user to show the history of commits. Finally Diff allows users to compare files between commits. 

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->
## Status
To check the status of the working directory for changes or additions:
```
git status
```
This will show you what untracked or modified files have and have not yet been staged.

## Log
Commits can be reviewed by using:
```
git log
```

**As depicted in the image below, each entry in the log shows:**
- The commit hash.
- Who made the commit.
- When it was made.
- Any commit messages made.

![a screen shot of an example of the commit message: Commit f2c87c8e (this hash is very long, as long as you have the first 8 digits you will be able to track it again) Author: Kyle Geske (userEmail) Date: Wed Sept 19 13:46:09 2018, (Commit message)"Added find_by and update_all to appropriate demo files"](GitLogExample.png)

The 40 character hex numbers shown at the start of each entry are the SHA1 hashes that uniquely identify each commit.


## Diff 
To compare the differences between the current files and the last commit:
```
git diff
```
We can diff specific files:
```
git diff secret_plans.txt
```
Or specific folders (and their sub-folders):
```
git diff ./textfiles/plans
```


## Sources and Additional Resources:

- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/01-version-control-tools/index.html#25)

- [Documentation of ```git status```](https://git-scm.com/docs/git-status)

- [Documentation of ```git log```](https://git-scm.com/docs/git-log)

- [Documentation of ```git diff```](https://git-scm.com/docs/git-diff)

- [Git Info Documentation](https://git-scm.com/docs/git)
