---
title: Forking Workflow
layout: default
parent: Team Git Workflow
nav_order: 3
---

<!-- prettier-ignore-start -->

# Forking Workflow
{: .no_toc }

The **Forking Workflow** is often used for open source projects. 

In this workflow, each developer gets not only their own local repository, but also a server-side copy of the project.

This allows for third-parties to work on a project without giving access to write on the original repository.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Strengths & Weaknesses of the Forking Workflow

**Strengths:**
- Developers push to their own server-side repositories.
- Changes are shared via pull requests from their personal public repository.
- The project maintainer has the final say on what is merged into the official repository.

**Weaknesses:**
- Difficult to see all active / inactive branches.
- Collaboration is trickier.

## Life Cycle of Forking Workflow

1. **Forking:** Each team member creates a fork of the project on the git hosting service.

2. **Cloning:** Team members clone their remote fork to a local repository.

3. **Adding an Upstream:** Team members configure a secondary remote called `upstream` that points to the official repository.

4. **Resolving Conflicts:** Remote commits from `upstream` can be pulled into the local feature branch, with merge conflicts resolved as required.

5. **Pushing to Remote:** Local feature branches are pushed to the forked remote.

6. **Requesting a Remote Merge:** Pull requests are initiated to request merges from the remote fork to the official upstream repository.

_**NOTE:** This workflow's life cycle is similar to the branching workflow, except instead of branching, you fork the repository._

## Sources and Additional Resources:

- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/03-git-team-collaboration/index.html#26)

- [Comparing Git workflows: What you should know](https://www.atlassian.com/git/tutorials/comparing-workflows)

- [Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)

- [Forking vs Branching in Github](https://stackoverflow.com/questions/3611256/forking-vs-branching-in-github)
