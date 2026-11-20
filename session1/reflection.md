# Session 1 Reflection
Muhammad Arif bin Saji (99895). All work was done using the Git command line (Git Bash on Windows).

## Q1. Why is a commit history useful when maintaining software?
A commit history records every change with its author, date and message, so I can see exactly what changed and why. If a bug appears, I can go back through the history to find the commit that introduced it and compare it with the version before. For example, in scm-lab-evidence my commits "Add student name to README" (2e96b3c) and "Add .gitignore" (f187e6b) are separate, so if the README broke I would know it changed in 2e96b3c and could inspect or undo only that change. Small commits with clear messages make maintenance much faster.

## Q2. Difference between Git and GitHub
Git is the version control program that runs on my computer; it created the repository, the commits and the session1-notes branch locally in scm-lab-evidence without needing the internet. GitHub is an online service that hosts Git repositories and adds collaboration features. My GitHub Skills exercise repository was created and worked on entirely on GitHub in the browser, using pull requests. My scm-lab-evidence repository was built with Git locally first, then pushed to GitHub so it is backed up and can be shared and cloned by others.

## Q3. What risk does working on a branch with a pull request reduce?
Working on a branch keeps main stable while changes are being made, so unfinished or broken work does not affect the main version. A pull request lets the changes be reviewed and checked before they are merged. This reduces the risk of introducing bugs or overwriting someone else's work on main. If something is wrong, the branch can be fixed or discarded without damaging main.

## Q4. Which commands changed only my computer and which changed GitHub?
Commands that changed only my computer: git init, git add, git commit, git switch, git merge, git branch -d, git restore and git remote add (it only saves the address locally). git clone and git pull downloaded from GitHub but only changed my local folders. Commands that changed GitHub: git push (including git push -u origin main), which uploaded my commits to the remote repository.

## Concept table (corrected against Appendix A)
| Term | Definition |
|---|---|
| Repository | A project folder plus its full history of changes. |
| Working tree | The files I can see and edit in my project folder. |
| Staging area (index) | The list of changes I have chosen to include in the next commit. |
| Commit | A saved snapshot of the project with a message, author and date. |
| Branch | A movable pointer to a line of commits, used to work in parallel. |
| Merge | Combining the work of two branches into one. |
| Remote | A copy of the repository on another server, for example origin on GitHub. |
| Push / Pull / Clone | Push uploads commits to the remote; pull downloads and integrates new commits; clone copies a remote repository for the first time. |

GitHub Skills exercise: https://github.com/arippp02/skills-introduction-to-github - branch my-first-branch, commit "Create PROFILE.md", pull request #2 (merged into main).
