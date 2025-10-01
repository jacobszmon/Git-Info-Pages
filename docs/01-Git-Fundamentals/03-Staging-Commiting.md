---
title: Staging and Committing
parent: Git Fundamentals 
nav_order: 3
---
<!-- prettier-ignore-start -->
# Staging and committing
{: .no_toc }

In order to properly use version control you need to commit your repository. However before you commit we must add our files to the staging area
## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->
## Staging Files Before we Commit
As we make changes to our code we **commit** the changes to our git repo. Before we can **commit** we must **add** new or changed files to a staging area.

**Let's stage our new readme.md file:**
```
git add readme.md
```
We could also use a period to stage all new or modified files:
```
git add .
```

Wilcards and sub-folders work too:
```
git add docs/textfiles/*.txt
```

## Committing Staged Files
We **commit** our staged changes with a commit message.
``` 
git commit -m "Your explanation of the changes goes here."
```

For complex changes, we can include a short title, followed by a long explaination:
```
git commit -m "Title" -m "Long description goes here .........."; 
```

We can even [configure git to open a text editor of our choice using:](https://docs.github.com/en/get-started/getting-started-with-git/associating-text-editors-with-git)


## Good Commit Messages are Crucial!
Quality commit messages contribute to:
- **Traceability**: Commit messages clarify code history and aid in debugging.
- **Collaboration**: They help others understand the intentions behind changes.
- **Documentation**: They act as a form of source code documentation.
- **Change Management:** "Change Logs" based on commits are often shipped with
each release.

**Examples of Good Commit Messages:**
- "Enhance user experience by validating sign up form fields."
- "Improve code readability by refactoring PlayerRegistrationService."
- "Prevent null reference crashes by adding pointer checks in the teleport code."

**Examples of Bad Commit Messages:**
- "fixing stuff"
- "Final version."
- "asdf"


Addition Notes:
[Class Notes](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531988/View)
[W3Schools Git Commit](https://www.w3schools.com/git/git_commit.asp)
[Git Documetation](https://git-scm.com/docs/git-commit)
