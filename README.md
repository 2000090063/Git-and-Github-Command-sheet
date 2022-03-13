
# Git and GitHub command cheat sheet

## init

Creating a local repository

```
$ git init
```

## clone

Copy the project from the remote repository

```
$ git clone [repository_path]
```

Copy the project by specifying the name of the directory you want to create

```
$ git clone [repository_path] [new repository_path]
```

Copy the project to get only the latest revision

```
$ git clone --depth 1 [repository_path]
```

## branch

Create branches

```
$ git branch [branch]
```

Display a list of branch

```
$ git branch
```

Display all branches

```
$ git branch -a
```

Display the remote branch

```
$ git branch -r
```

Delete the branch

```
$ git branch -d [branch]
```

## checkout

Switch the branch

```
$ git checkout [branch]
```

Switching to create a branch

```
$ git checkout -b [branch]
```

## diff, status

Display the differences of changed files

```
$ git diff
```

Display a list of changed files

```
$ git status
```

## add

Registration files and directories to index

```
$ git add [filename]
```

Register the changed files from the file that it has committed to the index

```
$ git add -u
```

Registered for all the modified file index  (file newly added is not included)

```
$ git add -A
```

Register all of the files and directories to index

```
$ git add .
```

## commit

Commit files that have been added to the index

```
$ git commit
```

Commit a file with the commit message

```
$ git commit -m "[comment]"
```

Commit to add to all the changed files index  (file newly added is not included)

```
$ git commit -a
```

Modify the last commit

```
$ git commit --amend
```

## log, show

Display the commit log

```
$ git log
```

Display the latest commit content

```
$ git show
```

## reset

Cancel the last commit  (the contents intact)

```
$ git reset --soft HEAD^
```

Cancel the contents and commit of the last commit

```
$ git reset --hard HEAD^
```

## push

Submit to commit the local repository to the remote repository

```
$ git push [remote] [branch]
```

Submit to commit the master of the local repository to the master of the remote repository

```
$ git push origin master
```

## pull-request

Send a pull request

```
$ git pull-request
```

Commit the file with the message of the pull request

```
$ git pull-request -m "[comment]" -b defunkt:master -h mislav:feature
```

## merge

Merge the branch

```
$ git merge [branch]
```

## fetch, pull

Confirm the change of the remote repository

```
git fetch [remote]
```

Incorporate a change in the remote repository

```
$ git pull [remote]
```

## cherry-pick

Copy the commit of another branch to the current branch

```
$ git cherry-pick [commit id]
```

## browse, open

Open a page of the project of GitHub

```
$ git browse
```
```
$ open https://github.com/USER_NAME/REPOSITORY_NAME
```

Open a page of the issues of the project of GitHub

```
$ git browse -- issues
```
```
$ open https://github.com/USER_NAME/REPOSITORY_NAME/issues
```

Opening the wiki pages of the project of GitHub

```
$ git browse -- wiki
```
```
$ open https://github.com/USER_NAME/REPOSITORY_NAME/wiki
```










