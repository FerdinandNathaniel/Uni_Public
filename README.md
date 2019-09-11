# Uni_Public

## Description

Public repository for uni assignments, primarily for coding assignments.

## Basic command line / git commands (Linux, most work in Windows or you can set up macros in order to do so)

`cd <dir>`: Stands for 'change directory', replace <dir> with the directory you want to 'go into'.

`ls`: Lists all contents of the directory you are currently in. Handy to find out where you are and where you can go.

`mkdir <dir_name>`: Makes a directory at the place you are at. Replace <dir_name> with the name you want the directory to have. You can't use spaces unless you surround the name with quotation marks.

`rm /path/to/file`: Removes a file. Path to file is relative to where you currently are (although you can also specify the entire path if you don't want to move around).

`git status`: Tells you the current status of the git directory you are in (whether files are staged, changed, removed, etc.)

`git pull`: Pull the files currently on the Git(Hub) repo to your local device (basically updates your local device to be in tune with what's available to everyone).

`git add <file>`: Add file to be 'staged'. Basically this means that a file you have edited is put up so it can be committed before being pushed towards the main branch (the online Git(Hub) repo).

`git add .`: Adds all file changes to be 'staged'. 

`git commit -m "message"`: Commits all staged files so they can be pushed to the main branch (online Git(Hub) repo). -m stands for 'message' and will be published next to your updates to make sense of what you just pushed.

`git commit -a -m "message"`: Adds all files to be staged and immediately commits them with the given message so they can be pushed to main branch. So -a stands for the 'git add .' command.

`git push`: Pushes your committed changes to the main branch.

`git branch`: Lists all current branches.

`git branch <branch_name>`: Create a branch with <branch_name>.

`git branch -d <branch_name>`: Delete the branch with <branch_name>.

`git checkout <branch_name>`: Check out <branch_name>. The main branch is called 'master'

`git checkout -b <branch_name>`: Create and immediately check out <branch_name>.

`git merge <branch_name>`: Merge <branch_name> with the branch you are currently on (which oftentimes means you need to be on 'master').

### Useful macros

Use TAB to automatically finish a filename or directory you are typing out (if it's present in your current dir).

Use CTRL(CMD)+SHIFT+C to copy and CTRL(CMD)+SHIFT+V to paste in the terminal.

Use CTRL+C to exit most terminal environments (like if you open jupyter notebook in the terminal, you can use CTRL+C (or ^C as it's shown in the terminal) to exit it)

### Example git (with branches)

just checking if everything's okay

`git status` 

create new branch and get on it
  
`git checkout -b test_branch`

commit some things you did

`git commit -a -m "added useless file"`

commit more things you did

`git commit -a -m "edited useless file"`

forget what branch you are on, or how the main branch is called 

`git branch`

go to main branch before merging your things you did

`git checkout master`

make sure you have the updated main branch before you merge

`git pull`

merge with main branch

`git merge test_branch`

delete now obsolete branch

`git branch -d test_branch`
