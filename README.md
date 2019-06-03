# git-notes

___

## Terminal Basics

* `~` is an alias for `$HOME` directory.

* `.` denotes the current directory.

* `..` denotes the parent directory.

* `*` is the wildcard symbol, selects all files in the working directory.

* Press the `tab` key for auto completion in the command-line.

* `less` is a program that displays the contents of a file.

* `cat` is a program that prints the contents of one of more files to the console.

* `mv` moves or renames a file or directory.

* `cp` copies a file or directory. Similar to `mv`, but `cp` leaves the original in-place. Must use the `-r` flag to recursively copy a directory.

* `rm` removes a file or directory. Use the `-r` recursive flag to remove a directory and its contents.

* `mkdir` creates a new directory. Use the `-p` flag to create nested directories. 

* `touch` creates a new file, but also used to update timestamps on a file.

* Use `command` + `K` to clear the terminal screen

 ___
 
 ## Branches
 
 * A branch is a version of the repository.
 
 * Each branch has its own commit history and current version.
 
`$ git branch` shows all branches.
 
`$ git branch my-branch-name` creates a new branch

`$ git branch -d some-old-branch` deletes the `some-old-branch`
 
`$ git checkout my-other-branch` switch to a new branch (checkout to a new branch) 
 
`$ git checkout -b my-branch-name` is the same as `git branch` and `git checkout` in one step

`$ git merge some-branch-name` merges the `some-branch-name` branch with the current working branch.

`$ git remote add origin https://github.com/Username/some-app.git`
The `origin` option is the default name for the server on which your remote repository is located.

Git doesn't care what you name your remote, but its typical to name your main branch `origin`.
 
 ___
 
 ## Configuration 
 
`$ git config --global user.name "John Doe"` sets a first and last name
 
`$ git config --global user.email "john-doe@gmail.com"` set the user email address
  
`$ git config --global color.ui true` turns on code highlighting
 
`$ git config --list` shows a list of all the set git configurations

`$ git init` initializes a hidden directory called `.git` in the project's root directory. "init"command stands for initialize.
 
 ___
 
 ## Adding files
 
`$ git add my-new-file.txt`
`$ git add my-new-file.txt other-file.js`
`$ git add .` adds all files in the current directory to the staging area
`$ git add -all` adds all the files in the root directory and other directories
 
`$ git rm --cached my-file-name` the `--cached` option indicats files in the staging area

`$ git rm -r folder-name` recursively removes all folders and files from the working directory

`$ git commit -m "Add three files to project"`

`$ git commit -am "Do something once more"` the `-a` option auto removes deleted files with the commit

`$ git reset my-file-name.js` removes a file form the staging area

`$ git reset --soft HEAD^` 

`--soft` option means that the commit is cancelled and moved before `HEAD`

You can now add another file to the staging area and commit, or you can amend files and commit them.

`HEAD` is just a pointer to a branch.

`^` represents the last commit


 
 
 
 
 


 
 
 
 
 
