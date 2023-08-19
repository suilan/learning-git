# Learning Git
Link: https://git-scm.com/docs. 

## Clonning Tips
Link: https://git-scm.com/docs/git-clone.

When you clone a repository, you get files and history from a remote repository to a new folder in the current directory that you're working on.

### Simple Clonning
Plain and simple clone repository to the current folder. This command will create a new folder called **learning-git/** at your pc.

``` bash
$ git clone https://github.com/suilan/learning-git.git
Cloning into 'learning-git'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
Receiving objects: 100% (3/3), done.
$ ls
learning-git

```

### Clonning repository with another name
Sometimes, when we clone an repository, we need to rename it.


``` bash
$ mkdir learning
$ cd learning
$ git clone https://github.com/suilan/learning-git.git git
Cloning into 'learning-git'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
Receiving objects: 100% (3/3), done.
$ ls 
git
```

### Clonning repository quietly
You can use *-q* or *--quietly* to hide progress. If there is an error, the terminal will show it.

``` bash
$ git clone -q https://github.com/suilan/learning-git.git git
$ ls 
git
```

### Clonning repository quietly
You can use *-v* or *--verbose* to see every step of the progress.

``` bash
git clone -v https://github.com/suilan/learning-git.git git
Cloning into 'git'...
POST git-upload-pack (175 bytes)
POST git-upload-pack (252 bytes)
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 8 (delta 0), reused 5 (delta 0), pack-reused 0
Receiving objects: 100% (8/8), done.
```





