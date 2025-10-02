---
title: Initializing Repositories
layout: default
parent: Git Fundamentals 
nav_order: 2
---
<!-- prettier-ignore-start -->
# Initializing Repositories 
{: .no_toc }

Creating repositories is the first and most important step when creating a new project. This is where we'll be storing, editing, and ultimately committing our files.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Repository Location
In order to make a repository, we first need a place to put it!

Let's make a folder to play in:
```
mkdir my-first-git
```
Next, let's move the terminal's focus into the folder we just made:
```
cd my-first-git
```


## Initializing Repositories
To bring a new project **under control** we must first initialize the repository (the repo) from within the project's root folder.

To initialize a new git repo from the command prompt: 
```
git init .
```

Note: Git defaults to using the word "master" ([as in "master copy" or "master recording"](https://git.github.io/rev_news/2020/07/29/edition-65/)) for the main branch, but we can change this:
```
git branch -m main
```


## Sources and Additional Resources:

- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/01-version-control-tools/index.html#24)

- [Git Documentation](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)

- [Data Camp](https://www.datacamp.com/tutorial/git-init)

