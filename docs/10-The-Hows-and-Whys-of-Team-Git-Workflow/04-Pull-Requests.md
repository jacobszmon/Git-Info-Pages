---
title: Pull Requests
parent: The How and Why of Team Git Workflow
nav_order: 4
---

<!-- prettier-ignore-start -->

# Pull Requests
{: .no_toc }

Without proper protocols and security measures, working collaboratively using GitHub can create more issues than it solves. 

**Pull Requests** can help to improve communication between team members about proposed changes, and provide a safety net against reckless merge attempts.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## What is a Pull Request?
**Pull Requests** are a mechanism to propose changes to a repo and facilitate discussion about them.

Pull requests are initiated prior to merging one branch with another branch of a project. The process involves comparing the two branches, detecting potential merge conflicts in advance so they can be resolved, and allowing for project administrators and potentially other contributors to:
- Review the changes.
- Comment on them.
- Suggest modifications.
- Approve or close the request.

**NOTE:** Pull requests are not part of git proper, they are instead facilitated by git hosting solutions like GitHub.

## Creating Pull Requests

**Step by Step Guide:**
1. Open the GitHub.com page for the repository.    

2. Once there, open the "Pull Requests" tab.

3. Click the "New Pull Request" Button at the top right.

4. Once there, you'll see a dropdown menu labelled "base repository", click it and ensure that you've chosen the proper repository.

5. Now you should see two dropdowns labelled "base" and "compare". 
    - Choose the branch you'd like to merge your branch into for "base".
    - Choose the branch you'd like to merge for "compare".
    
6. Hit the green "Create Pull Request" button.

7. Fill out Title and Description.
    - Write a clear and concise Title for your request.
    - Write a description that clearly communicates the desired changes from your branch.
    
8. Once finished, press the "Create Pull Request" button once again, and your pull request is now finished.



**NOTE:** Git GUIs (like Visual Studio or GitHub Desktop) will often provide you with a link to create a request after pushing changes to a remote branch. Though often their capabilities in doing so are quite limited.



## Pull Request Merge Conflicts

You will be prevented from creating a pull request if your branch can't be merged.

**To resolve the conflict:**
1. Locally checkout the `main` branch.

2. Pull the latest changes into `main` from the remote.

3. Checkout your branch. (The one you wanted to merge.)

4. Merge `main` into your branch.

5. Resolve the conflicts using your editor or merge tool.

6. Commit your changes to your branch.

7. Push your branch to the remote.

8. Attempt to create the pull request again.

## Source & Additional Links

- [Class Notes on Pull Requests](https://stungeye.github.io/Software-Development-And-Documentation-1/03-git-team-collaboration/index.html#28).

- [About Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
