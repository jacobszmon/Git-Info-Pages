---
title: Reset
layout: default
parent: Undoing in Git with
nav_order: 2
---

<!-- prettier-ignore-start -->
# Reset
{: .no_toc }

Reset is a git command that provides a dangerous and potentially destructive way to undo commits in a git repository.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## What is Reset?

A git reset comes in three flavors, each affecting the repository differently:
- **Hard Reset (Dangerous)**: Resets the HEAD pointer, staging area, and your working directory to match a specific commit. All uncommitted changes are lost when they are reset to the specified commit.

- **Mixed Reset (Weirder)**: Resets the HEAD pointer and the staging area, but keeps the changes in your working directory. The HEAD and your working directory may differ if you had uncommitted changes.

- **Soft Reset (Weird)**: Resets the HEAD pointer, but keeps the changes in the staging area and working directory. The HEAD and your working directory may differ if you had uncommitted changes.

_⚠️ **WARNING**: Using ```git reset``` is dangerous. It rewrites your repository's history by changing the HEAD pointer. Commits after the reset point are not "lost", but they can become difficult to recover._



## How to use Reset

To do a Hard Reset: 
```
git reset --hard [commit id]
```


To do a Soft Reset: 
```
git reset --soft [commit id]
```


To do a Mixed Reset: 
```
git reset --mixed [commit id]
```

To look at work in an old commit, before returning to where you were:
```
// reset to commit B
git reset --hard [B] 

// reset back to commit D
git reset --hard [D] 
```

## Sources and Additional Resources:
- [Class Notes on ```git reset```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#6)
- [Documentation for ```git reset```](https://git-scm.com/docs/git-reset)
- [An explanation of ```git reset``` including Mixed Resets](https://practicalseries.com/1002-vcs/02-05-concept.html#js--020505)
