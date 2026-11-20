# Session 2 Reflection
Muhammad Arif bin Saji (99895). All local work was done using the Git command line (Git Bash).

## Q1. How do Issues and pull requests together support change control?
The Issue records why a change is needed and how to tell when it is done, through acceptance criteria. The pull request carries the actual change from a branch and the review discussion. By writing "Closes #1" in PR #2, the change was linked to its reason, and the issue closed automatically when the PR was merged. This gives a full chain from request to review to merge that anyone can follow later.

## Q2. Why did the conflict in Part 4 happen, and how could a team reduce such conflicts?
The conflict happened because branch-a and branch-b were both created from the same version of main and both changed the same line of session2/conflict-demo.md, to "staging" and "production". After branch-a was merged, Git could not decide automatically which version of that line to keep when merging branch-b. A team can reduce conflicts by pulling often, keeping branches short-lived and small, and agreeing who works on which files. Communicating through Issues also helps avoid two people changing the same thing.

## Q3. What would be lost if people merged straight into main without a pull request?
There would be no review step, so mistakes, bugs or secrets could go straight into the main version. The discussion and reasoning behind each change would not be recorded, and changes would not be linked to their Issues. This would make it much harder to trace why something changed, and to find and undo a bad change later.
