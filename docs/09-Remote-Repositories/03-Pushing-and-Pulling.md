---
title: Pushing and Pulling
parent: Remote Repositories
nav_order: 2
---

<!-- prettier-ignore-start -->

# Pushing and Pulling
{: .no_toc }

Pushing and Pulling are the two main commands to using a remote repository.

This module will teach you the GitHub workflow and also the best practices of pushing and pulling.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## GitHub Workflow

If you want to make a copy of a GitHub repository to your local machine, you can **clone** it:

```
git clone git@github.com:<INSERT-YOUR-GITHUB-USERNAME>/<INSERT-YOUR-REPOSITORY-NAME>.git
```

Once you have your local and remote repository set up, you can **push** and **pull** changes.

## Pushing

When you want to send your commits of the local repository to GitHub:

```
git push origin <INSERT-YOUR-BRANCH-NAME>
```

With this command your local commits on the repository will be sent to the GitHub repository.

This links all your changes to the remote repository, but not your future changes, you must push whenever you wish to send a change.

Think of it as making documents that you then fax over to your office.

## Pulling

When you want to grab the latest commits from your remote repository on GitHub:

```
git pull origin <INSERT-YOUR-BRANCH-NAME>
```

If your repository is not updated to the current state of the remote repository, pulling will update your local repository.

It is best practice to pull before pushing to avoid merge conflicts.

**Important:** If you made any commits on your local repository before pulling, you may run into **merge conflicts** that you have to resolve.