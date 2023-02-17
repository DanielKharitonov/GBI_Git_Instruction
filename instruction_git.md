# Instruction git 

![logo](logo.jpeg)

_**Git** - is system for monitoring file versions._ 
Program saves every change with comment. She saves difference. When you want to open file version, program loads source file and adds into the file change the version.

## Repository

*It is file versions (file changes) storage.*

Enter command to create new repository into the present folder:

    git init

Enter command to see status repository:

    git status

## Adding change to tracking

Enter command to index a change:

    git add <fale_name>

This means, you want add a change to next commit

## Commit change

Enter command to commit a chenge:

    git commit

*When text editor (installed by default) will open, enter comment to change and exit from text editor*

If you want to enter comment in terminal, enter command:

    git commit -m "you comment"

If you want to index all changes (execute command git add) and to commit the chenge, enter command:

    git commit -a

*When text editor (installed by default) will open, enter comment to change and exit from text editor*

If you want to index all changes (execute command git add), to commit the chenge and to enter comment in terminal, enter command:

    git commit -am "you comment"

## Log commits (changelog)

Enter command to show log commits present branch with full info (author, date, message):

    git log 

If you want see shortlog commits present branch, enter command:

    git log --oneline

If you want see log commits all branches with full info (author, date, message, enter command):

    git log --all

If you want see shortlog commits all branches, enter command:

    git log --oneline --all

If you want see in terminal shortlog commits all branches in simple graphic form, enter command:

    git log --oneline --all --graph

## Moving through commits and branches

Enter command to move to commit with index "hash":

    git checkout <hash>

*After command you will see your file change with index "hash"*

Enter command for return:

    git checkout <name main branch>

Or enter command with index next commit, what you want see.

If you want to go to another branch, enter command:

    git checkout <branch_name>

## Viewing the changes

Enter command to show changes between last commit and present file:

    git diff

If you want see changes between commits with index "hash1" and "hash2", enter command:

    git diff <hash1> <hash2>

## Branching

*Branching uses for collaborate on the file or changes on the file while another users use this file.*

Enter command to create new branc:

    git branch <branch_name>


If you want delete branch, enter command with option:

    git branch -d <branch_name>

*But before that, you will need to execute merging branches*

## Merge one branch wit another branch 

For merging another branch wit your branch (where you are), enter command:

    git merge <branch_name>

*After that there may be a conflict, that you need to solve*

## Merging conflict

Merge conflicts occur when competing changes are made to the same line of a file, or when one person edits a file and another person deletes the same file.

To resolve a merge conflict caused by competing line changes, you must choose which changes to incorporate from the different branches in a new commit.

1. Open your text editor and navigate to the file that has merge conflicts.
2. When you open the file in your text editor, you'll see the changes from  base branch after the line <<<<<<< HEAD. Next, you'll see =======, which divides your changes from the changes in the other branch, followed by >>>>>>> BRANCH-NAME. 
3. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge. 
4. Add or stage your changes.
5. Commit your changes with a comment.

## Remote repositories

Remote repositories are versions of your project saved on the Internet. You can have several remote repositories.

Repository management includes both the ability to add new repositories and the ability to delete outdated repositories, as well as the ability to manage various remote branches, declare them tracked or not, and so on.

### Git Clone

The command is used to create a copy of a specific repository or branch within a repository.

When you clone a repository, you don't get one file, like you may in other centralized version control systems. By cloning with Git, you get the entire repository - all files, all branches, and all commits

Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits:

    git clone [url]

### Git Pull

git pull updates your current local working branch, and all of the remote tracking branches. It's a good idea to run git pull regularly on the branches you are working on locally.

Without git pull, (or the effect of it,) your local branch wouldn't have any of the updates that are present on the remote.

Update your local working branch with commits from the remote, and update all remote tracking branches:

    git pull

### Git push

Uploads all local branch commits to the corresponding remote branc:

    git push


