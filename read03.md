
# Read 03 Notes

This is is tougher subject for me to learn, but I am slowly learning how to use the git from the terminal.

## Centralized Version Control or CVS
This system is a single server storing all changes and file versions, accessible to various users. 

## Distributed Version Control System or DVCS
This allows multiple repositiories so each team member has a copy to work with. This ensures that data will not be lost since it is stored in multiple locations, most likely each individual's local. This is a good safety net over the CVS to ensure the files will be safe if the CVS has a critical failure and loses all files.

## Local Repo Structure - there are three components
1. Working directory - The actual files reside here
2. Index - The area used for staging
3. Head - The most recent commit

## Tracked vs Untracked
- Tracked files can be modified, unmodified, or staged. These were part of the most recent snapshot.
- Untracked files were not in the last snapshot and aren't currently in staging area.
1. After you edit a file, Git flags it as modified
2. You stage the modified file
3. Then commit staged commands

### Here is a list of things you need to know
# ACP. or Add, Commit, Push
- git add file - this will add a file
- git commit - this will commit any changes to the file
- git push - this will commit changes to github

The above commands are extremely important. Here are some more:
- git init - This command initializes existing repo
- git commit -m "any message here" - to add a note regarding possible changes
- git clone url of website - by cloning, you will have copied all versions of all files for a project. This will creat a dir. called "test" with a .git directory inside, which has all the files copied.
- git clon url mydirectory - makes a copy of target repo in a target directory, so mydirectory.
- code . - to access my VScode
- git status - to check the state of files
- git add filename - track one file in repo
- git add * - track all files in repo
- git commit -m "changes xyz" - to add message of commited changes. These are commited to the HEAD
- git command -a - commit all changes
- git push origin main - this will push changes from main to remote repo names origin
- git stash - save changes but not commit. these will be hidden. to find them, type git stash apply to find them.
- git stash apply - to find stashed files you haven't yet commited
- git remote - to view shortnames
- git remote -v - to view remote urls
- touch - to create a file
- rm - to remove files

These are the most basic ones and should get you through the basics. You can always check into [Git Intro](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#1)


[Back to home](README.md)

https://skylerjohnson102020.github.io/reading-notes/read03.html
