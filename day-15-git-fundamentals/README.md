📌Day 15 – Git Fundamentals

Objective

Learn the fundamentals of Git, initialize a local repository, track file changes, stage files, create commits, and review commit history.

Topic 1: Introduction to Git

Git is a version control system used to track changes in files and maintain project history.

What I Learned

- Git tracks changes over time.
- Git helps maintain a history of project updates.
- Git and GitHub are different: Git is the version control tool, while GitHub hosts Git repositories online.

Topic 2: Git Repository

Command practiced:

git init

What I Learned

- "git init" initializes a new local Git repository.
- Git creates a hidden ".git" directory to store repository information.
- I initialized a repository in "git-day15-practice".

Topic 3: Checking File Changes

Commands practiced:

git status
echo "Learning Git fundamentals" > notes.txt

What I Learned

- "git status" displays the current repository state.
- "notes.txt" initially appeared as an untracked file.
- Git can identify files that have not yet been committed.

Topic 4: Staging and Committing

Commands practiced:

git add notes.txt
git status
git commit -m "Add Git practice notes"

What I Learned

- "git add" stages file changes for a commit.
- The staging area lets me select which changes to include in the next commit.
- "git commit" records a snapshot of the staged changes.
- I configured my Git name and email to identify my commits.

Topic 5: Git History

Command practiced:

git log -1 --oneline

What I Learned

- "git log" displays commit history.
- "--oneline" presents each commit in a compact format.
- My first commit was created successfully.

Commit Details

- Commit message: "Add Git practice notes"
- Commit ID: "518b72e"

Tools Used

- Kali Linux
- Linux terminal
- Git

Key Takeaways

- Initialize a Git repository.
- Check repository status.
- Stage files and create commits.
- Review commit history.
- Understand the difference between Git and GitHub.

Status

Day 15 – Git Fundamentals: Completed.

Note: This practice repository is stored locally. It has not been uploaded to GitHub.
