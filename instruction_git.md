# Instruction for working with git program

_**Git** - is system for monitoring versions file._ 
Program saves every change with comment. She saves difference. When you want to open version file, program loads source file and adds into the file change the version.

## Repository

*It is file versions storage (file changes).*

Enter comand to create new repository  into the present folder:

    git init

Enter comand to check status repository:

    git status

## Adding change to tracking

Enter comand to index the change:

    git add <fale_name>

This means, you want add the change to next commit

## Commit change

Enter comand to commit the chenge:

    git commit

*When text editor (installed by default) will open enter comment to change and exit from text editor*

If you want to enter comment in terminal, enter command:

    git commit -m "you comment"

If you want to index the change (execute command git add) and to commit the chenge, enter comand:

    git commit -a

*When text editor (installed by default) will open enter comment to change and exit from text editor*

If you want to index the change (execute command git add), to commit the chenge and to enter comment in terminal, enter comand:

    git commit -am "you comment"

## Log commits (changelog)

Enter comand to show log commits present branch with full info about author, date, message:

    git log 

If you want see shortlog commits present branch, enter comand:

    git log --oneline

If you want see log commits all branches with full info about author, date, message, enter comand:

    git log --all

If you want see shortlog commits all branches, enter comand:

    git log --oneline --all
   