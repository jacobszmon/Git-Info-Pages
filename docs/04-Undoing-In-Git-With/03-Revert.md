---
title: Revert
parent: Undoing in Git with
nav_order: 3
---

<!-- prettier-ignore-start -->
# Revert
{: .no_toc }

Revert is a git command that provides a safe, public way to undo commits in a git repository.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## What is Revert?
Revert creates a new commit that undoes changes from the specified commit, essentially performing a reverse commit.

Reverting maintains history, which makes it a safe choice for undoing local commits and undoing commits pushed to a remote repository. You can think of it as a public undo, saying *"I made a mistake, but I want to keep a record of it."*



## How to use Revert
To create a new commit that undoes changes from the specified commit:
```
git revert <commit id>
```
NOTE: ```git revert``` reverts a single commit by default. In the following examples, uppercase letters (C, D, etc.) are commit IDs in sequence with one another.

To revert multiple commits, you can revert the commits individually, working backwards:
```
git revert D
git revert C
git revert B
```
OR, you can revert a sequence of commits: *(Using this method, each commit is reverted separately.)*
```
git revert B^..D
```
If you only want a single revert commit: *(The -n stands for "no commit".)*
```
// cancel revert's automatic commit using -n
git revert -n B^..D 

// then perform a commit manually to only commit once.
git commit -m "Revert commits C through D inclusively." 
```

## Sources and Additional Links
- [Class Notes on ```git revert```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#11)
- [Documentation for ```git revert```](https://git-scm.com/docs/git-revert)
