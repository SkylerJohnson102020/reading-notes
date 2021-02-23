# Read 03 Notes

This is is tougher subject for me to learn, but I am slowly learning how to use the git from the terminal.

## Centralized Version Control
This system is a single server storing all changes and file versions, accessible to various users. 





##Local Repo Structure - there are three components
1. Working directory - The actual files reside here
2. Index - The area used for staging
3. Head - The most recent commit


### Here is a list of things you need to know
ACP. or Add, Commit, Push
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

These are the most basic ones and should get you through the basics. You can always check into [Git Intro](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#1)


[Back to home](README.md)

https://skylerjohnson102020.github.io/reading-notes/read03.html
