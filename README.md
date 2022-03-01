# Introduction to Git
- [Installing git](#installing-git)
- [Git useful commands](#git-useful-commands)
- [More about git](#more-about-git)

## Installing git
you can install git from [here](https://git-scm.com/downloads)<br/>
to be sure that git has been installed you can use `git --version`

## Git useful commands
**git config**
- **`git config --global user.name "(name)"`**
  > usage : setting name for commits<br/>
  > example : `git config --global user.name "Javad"`
  
- **`git config --global user.email "(email)"`**
  > usage :  setting email address for commits<br/>
  > example :  `git config --global user.email "name@gmail.com"`

**git init**
- **`git init (repository name)`**
  > usage : creating an empty local git repository<br/>
  > example : `git init /home/javad/projects/chessGame`

**git clone**
- **`git clone (url)`**
  > usage :  to clone a repository into a newly created directory<br/>
  > example : `git clone https://github.com/JavadZandiyeh/LearningGit`

**git add**
- **`git add (file name)`**
  > usage : adding file to Staged area<br/>
  > example : `git add testFile.html`
  
- **`git add -A`** or  **`git add *`**
  > usage : adding all files to Staged area
  
- **`git add *.(file type)`**
  > usage : adding all files (with this file type) to Staged area<br/>
  > example : `git add *.java`

**git commit**
- **`git commit`**
  > usage : committing all files which are in Staged area<br/>
  > *note* : this command open's a text editor for you and you have to write your message on
 
- **`git commit -m "(your message)"`**
  > usage : committing all files which are in Staged area<br/>
  > example : `git commit -m "Adding top menu bar"`

**git status**
- **`git status`**
  > usage : show status of files![alt text](https://github.com/JavadZandiyeh/LearningGit/blob/master/pict.png?raw=true)
  
**git log**
- **`git log`**
  > usage : show history of current branch

**git diff**
- **`git diff HEAD`**
  > usage : show all changes to tracked files
  
- **`git diff --staged`**
  > usage :  show changes to files in the Staged area

**git reset**
- **`git reset (file name)`**
  > usage : putting files (which are in Staged area) to Untracked area<br/>
  > example : `git reset pict.png`

**git branch & git checkout & git merge**
- **`git branch`**
  > usage : show all branches

- **`git branch (name of branch)`**
  > usage : creating a new branch by this name<br/>
  > example : `git branch developer`

- **`git branch -d (branch name)`**
  > usage : deleting branch if exists<br/>
  > example : `git branch -d developer`

- **`git checkout (branch name)`**
  > usage : changing branch<br/>
  > example : `git checkout developer`

- **`git checkout -b (branch name)`**
  > usage : creating a new branch by this name and also changing your branch to this branch<br/>
  > example : `git checkout -b GUI` 

- **`git merge (branch name)`**
  > usage : merging this branch into the current branch<br/>
  > *note* : if you want to merge a branch into the master you have to checkout to master branch and then use this command<br/>
  > example : `git merge GUI` 
 
**git remote**
   - **`git remote add origin (url of repository)`**
     > usage : connecting your local repository to the remote server by this url<br/>
     > example : `git remote add origin https://github.com/JavadZandiyeh/LearningGit`

**git tag**
- **`git tag`**
  > usage : show all tags

- **`git tag -a (tag name) -m "(your message)"`**
  > usage : creating a new tag for last commit<br/>
  > example : `git tag -a version3.4 -m "this is version 3.4"`

- **`git tag -a (tag name) (hash of commit) -m "(your message)"`**
  > usage : creating a new tag for commit by this hash<br/>
  > example : `git tag -a version3.1 729375b1d1eaad8a2fb559a2ce4fc8a70d52c74a -m "version 3.1 for unveiling"`
 
 **git show**
 - **`git show (hash of commit)`**
   > usage : show changes of this commit<br/>
   > *note* : you can find hash of commits by `git log` command<br/>
   > example : git show 729375b1d1eaad8a2fb559a2ce4fc8a70d52c74a
  
  - **`git show (name of tag)`**
    > usage : show commits of this tag<br/>
    > example : `git show problemForLogic`

**git push**
- **`git push origin (branch name)`**
  > usage : pushing the local branch into the remote server(can be github, gitlab or etc)<br/>
  > example : `git push origin master`
 
 - **`git push origin --tags`**
   > usage : pushing all new tags into the remote server
 
 - **`git push origin (tag name)`**
   > usage : pushing this tag into the remote server<br/>
   > example : `git push origin version3.4`

**git pull**
- **`git pull origin (branch name)`**
  > usage : pulling branch from remote server(can be github, gitlab or etc) into the local branch<br/>
  > example : `git pull origin logic`

## More about git
- README files :  [stackedit.io](https://stackedit.io/)
- more about commands : [git-scm.com/docs](https://git-scm.com/docs)
