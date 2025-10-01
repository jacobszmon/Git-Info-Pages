---
title: Feature Branch Workflow
parent: The How and Why of Team Git Workflow
nav_order: 2
---

<!-- prettier-ignore-start -->

# Feature Branch Workflow
{: .no_toc }

The **Feature Branch Workflow** is about working feature development or bug fixes on dedicated branches for each feature / fix.

Team members are divided to work on each feature in those branches and minimizes merge conflicts.

The main branch is always kept clean and branches are only pulled into main when it is finished.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Strengths & Weaknesses of the Feature Branch Workflow

These are the strengths and weaknesses of the Feature Branch Workflow.

Strengths:
- Isolates new development from the main branch.
- Makes it easy to discard experimental changes.
- Facilitates code review via pull requests.

Weaknesses:
- Not all developers are updated on each branch when working with multiple feature branches.
- Unnecessary Merge Conflicts may arise.
- Long branches require long reviews.

_**Note:** This workflow is sometimes called [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow)._

## Life Cycle of Feature Branch Workflow

1. **Branching:** New features or fixes are developed locally in a short-lived branch.

2. **Resolving Conflicts:** Remote commits by other developers can be pulled into the local feature branch, with merge conflicts resolved as required.

3. **Pushing to Remote:** Completed and resolved branches are then pushed.

4. **Requesting a Remote Merge:** A pull request is next initiated on the git hosting service (example; GitHub).

5. **Reviewing:** One or more team members review the pull request before merging it into the main remote branch.

_**Note:** Pull requests can be sent back unmerged if rework is deamed necessary._

## Source & Additional Links

[Class Notes](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).

[Comparing Git workflows: What you should know](https://www.atlassian.com/git/tutorials/comparing-workflows).

[Git Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow).

[The Pitfalls of Feature Branching](https://www.cloudbees.com/blog/pitfalls-feature-branching).