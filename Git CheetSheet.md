

![download](/Users/jonny/Downloads/download.png)



### 1. What is git?

- An open source, distributed version-control system

### 2. What is GitHub?

-  A platform for hosting and collaborating on Git repositories

### 3. Commit?

- A snapshot of your entire repository 
- Compressed into a SHA

### 4. Branch?

-  Allows you to duplicate the source code for yourself. You will then work on your own branch so your edits do not immediately affect the original source code.

### 5. Clone?

- A local version of a repository, including all commits and branches

### 6. Remote?

- A common repository on GitHub that all team member use to exchange their changes

### 7. Fork?

-  A copy of a repository on GitHub owned by a different user

### 8. Pull request?

- A place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more

### 9. HEAD?

-  Representing your current working directory, the HEAD pointer can be moved to different branches, tags, or commits when using `git checkout`

### 10. Merging?

- The process of joining your branch with the original source code after complete testing.



### How to setup git for the first time?

###### Generating the ssh key (Only required to establish secured connection between local machine and github)

- ssh-keygen -t rsa

###### Validating the proper establishment of secured connection

- ssh -T git@github.com

/c/Users/username/.ssh/id_rsa.

```
- Downaload git accoding to your local machine - https://git-scm.com/
- git config user.name or user.email  (Check if any userName is there or not)
- git config --global user.name "[name]"
- git config --global user.email "[email address]"
- git init
- git clone
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin (https://github.com/----)
- git push -u origin main
```



### Push an existing repository 

```
git remote add origin (https://github.com/.git)
git branch -M main
git push -u origin main
```



## Here is a few command you will use everyday:

```
- git clone
- git pull origin master
- git checkout -b new_branch_name
- git add file_name 
	- git add . --adding all files
	- git add * --adding all files
- git status
- git log
- git commit -m "What changes did you make?"
- git push branch_name
- git pull origin master
- git commit --amend   (commit again using the --amend option --- you make the additional changes you forgot, stage them)
- git reset HEAD File_name (to unstage)
- qa!  and ENTER --(to close vim) -- if you forget to commit the msg & VIM opened. 
```



## How to configure 

1. Sets the email you want attached to your commit transactions

   ```
   git config --global user.email "[email address]"
   ```

2. Sets the name you want attached to your commit transactions

   ```
   git config --global user.name "[name]"
   ```

3. Enables helpful colorization of command line output

   ```
   git config --global color.ui auto
   ```



##  How to create Branches

1. Creates a new branch

   ```
   git branch [branch-name]
   ```

2. Switches to the specified branch & Updates

   ```
   git checkout [branch-name]
   ```

3. Combines or merge from your current branch to main/master branch, done by pull requests

   ```
   git merge [branch]
   ```

4. Deletes the specified branch

   ```
   git branch -d [branch-name]
   ```



## How to create repositories

1. Turn an existing directory into a git repository

   ``` 
   git init
   ```

2. Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

   ```
   git clone [url]
   ```



## .gitignore - Exclude files

- Exclude files from being tracked with Git. 
- Create special file named `.gitignore` . 



## How to synchronize changes

1. Uploads all local branch commits to GitHub

   ```
   git push
   ```

2. Get the latest code on your local branch. git pull is a combination of git fetch and git merge

   ```
   git pull
   ```

3. Combines remote tracking branch into current local branch

   ```
   git merge
   ```

4. Downloads all history from the remote tracking branches

   ```
   git fetch
   ```



## Make changes

1. Snapshots the file in preparation for versioning

   ``` 
   git log
   ```

2. git add [file]

   ```
   git add [specific file]
   git add . ---> adding all files
   ```

3. Records file snapshots permanently in version history

   ```
   git commit -m "[descriptive message]"
   ```

4. Lists version history for a file, including renames

   ```
   git log --follow [file]
   ```

5. Shows content differences between two branches

   ```
   git diff [first-branch]...[second-branch]
   ```

6. Outputs metadata and content changes of the specified commit

   ```
   git show [commit]
   ```



## Redo commits

1. Undoes all commits after [commit], preserving changes locally

   ```
   git reset [commit]
   ```

2. Discards all history and changes back to the specified commit

   ```
   git reset --hard [commit]
   ```



















---

## QA

---

###### 1. How to check git version?

- Git --version

###### 2. How to configure for the first time?

- git config --global user.name "Name"
- git config --global user.email "Email"

###### 3. How to get help from git?

- Git config --help
- Git add --help
- Git commit --help

######  4. How to create a new local repository and initialize it to a git repository?

- git init

###### 5. How to clone or download from GitHub?

- git clone (url)

###### 6. How to find the local code chanage or status?

- git status

###### 7. Add Files to staging area

- git add abc.txt --one file
- git add . or *  ---all files
- git add - A.  --all files

###### 9. Commit the changes

- git commit -m "first commit"

###### 10. For forcefully reverting the previous commit

- ```
  git reset --hard
  ```

- ```console
  git commit --amend
  ```

###### 11. For clearing the changes in local / revert the changes?

- git stash

###### 12. How to Tracking the commits?

- git log

###### 13. Which remtoe repository are we connected with? View information about remote repository

- git remote -v

###### 14. How to send changes to the master brach

- git push origin master

###### 15. How to get latest update from the remote repository?

- git pull
- git pull origin master

###### 16. How to pull from remote branch?

- Pull a remote branch:

###### 17. Reset the added files back to working directory

- git reset
- git reset abc.txt

###### 18. How to know what branch I am in?

- git branch

###### 19. How to switch or checkout from branches?

- $ git checkout <branchname> 

###### 20. How to merge the branches?

- git merge <branch name>

###### 21. How to create a branch?

- git branch <branch name>

###### 22. How to undo changes?

- git revert  OR $ git revert **<****commit-ish****>** 

###### 23. How to remove the files?

-  Git rm  OR $ git rm <file Name>

###### 24. Remove files from the Git But keep the files in your local repository:

- $ git rm --cached

###### 25. Finding the changes made

- git diff
