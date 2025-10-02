---
title: Git Ignore
layout: default
parent: Git Fundamentals 
nav_order: 5
---
<!-- prettier-ignore-start -->
# Git ignore
{: .no_toc }

Sometimes we don't need certain files taking up storage in our repository. We use Git ignore to combat this. By simply putting a file called .gitignore we are able to exclude specific file types. 

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->
## Not Every File Should Be Included
Sometimes there are files you don't want to include in your repo:
- Files that include secrets like passwords or API keys.
- Temporary files and folders.
- Build files and folders.
- Hidden OS files like .DS_Store (Mac) or Thumbs.db (Windows) files.

Handy:[ Useful .gitignore templates for common languages and technologies.](https://github.com/github/gitignore) 

## Git Ignore File
Exclude files and folders by create a ``.gitignore`` file in the project root:
Ignore specific files.
```
# This is a comment in the ignore file

# Ignore a specific file (in this case Thumbs.db)
Thumbs.db

# Wildcards: Ignore all .exe files.
*.exe

# Exception to wildcards: Track the special.exe file, even though we aren't tracking .exe files.
!special.exe

#Ignore all files in any folder called build.
build/

# Ignore all .pdf files in the doc/ folder and any of its sub-folders.
doc/**/*.pdf
```


## Sources and Additional Resources:

- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/01-version-control-tools/index.html#33)

- [Git Ignore GitHub Docs](https://docs.github.com/en/get-started/git-basics/ignoring-files)

- [Git Documentaion](https://git-scm.com/docs/gitignore)
